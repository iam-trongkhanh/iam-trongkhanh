<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Khanh Trong Le (Lê Trọng Khánh). Cloud and DevOps labs on AWS, Ho Chi Minh City, UTC+7. Lab delivery path: commit, check and build, publish to ECR, Argo CD sync, run on EKS." src="assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://khanhcloud.online/"><img alt="Portfolio: khanhcloud.online" src="https://img.shields.io/badge/khanhcloud.online-252026?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA5NiA5NiI%2BPHBhdGggZmlsbD0iI0U1RjQ4MSIgc3Ryb2tlPSIjMjUyMDI2IiBzdHJva2Utd2lkdGg9IjIuNSIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgZD0iTTI0IDgyQzEyIDgyIDQgNzMgNCA2MkM0IDUxIDExIDQzIDIyIDQxQzIzIDIzIDM0IDEyIDQ5IDEyQzY0IDEyIDc2IDIyIDc5IDM3Qzg3IDM5IDkzIDQ2IDkzIDU2QzkzIDcwIDgzIDgyIDY5IDgyWiIvPjxwYXRoIGZpbGw9IiMyNTIwMjYiIGQ9Ik0yNyA4MkwzNiAzN0g0OUw0NSA1N0w2NSAzN0g4MUw1NiA2Mkw3MyA4Mkg1Nkw0MiA2NkwzOSA4MloiLz48L3N2Zz4%3D"></a>
  <a href="https://www.linkedin.com/in/trongkhanh-cloud/"><img alt="LinkedIn: trongkhanh-cloud" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge"></a>
  <a href="mailto:le.trongkhanhqlv@gmail.com"><img alt="Email: le.trongkhanhqlv@gmail.com" src="https://img.shields.io/badge/Email-575126?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

<p align="center"><b>Open to junior and associate Cloud &amp; DevOps roles, including remote (UTC+7).</b></p>

---

I build university and personal Cloud/DevOps labs on AWS and write each one up as a **case file**: the problem, the exact Terraform or pipeline lines at a pinned commit, and a scope note that separates what was applied from what is design. The labs cover Terraform for Amazon EKS networking, Jenkins → Argo CD delivery and private S3 for build artifacts. OrderFlow, a containerised order API, is the one I am taking to AWS next.

## Case files.

<table>
<tr>
<td width="50%" valign="top">

### AWS DevSecOps delivery lab
<img alt="Jenkins" src="https://img.shields.io/badge/Jenkins-252026?style=flat-square&logo=jenkins&logoColor=E5F481"> <img alt="Terraform" src="https://img.shields.io/badge/Terraform-252026?style=flat-square&logo=terraform&logoColor=E5F481"> <img alt="Amazon EKS" src="https://img.shields.io/badge/Amazon_EKS-252026?style=flat-square&logo=kubernetes&logoColor=E5F481"> <img alt="Argo CD" src="https://img.shields.io/badge/Argo_CD-252026?style=flat-square&logo=argo&logoColor=E5F481">

- Parameterised Jenkins pipeline for Terraform `init` / `validate` / `plan` / `apply` / `destroy`
- EKS module inputs for networking, node capacity, cluster access and add-ons
- Argo CD Application declared with automated prune and self-heal
- Scope: university architecture lab; configuration, not a recorded rollout

**[Read the case file →](https://khanhcloud.online/work/aws-devsecops/)** · [Repository](https://github.com/iam-trongkhanh/End-To-End-K8s-Devops-Project)

</td>
<td width="50%" valign="top">

### Amazon EKS with Terraform
<img alt="Terraform" src="https://img.shields.io/badge/Terraform-252026?style=flat-square&logo=terraform&logoColor=E5F481"> <img alt="Amazon EKS" src="https://img.shields.io/badge/Amazon_EKS-252026?style=flat-square&logo=kubernetes&logoColor=E5F481"> <img alt="Amazon VPC" src="https://img.shields.io/badge/Amazon_VPC-252026?style=flat-square"> <img alt="IAM" src="https://img.shields.io/badge/IAM-252026?style=flat-square">

- Separate VPC, EKS, managed node group and IAM modules
- Private worker subnets; NAT egress shared or one per Availability Zone
- KMS for Kubernetes Secrets, control-plane logs, OIDC provider for IRSA
- Scope: infrastructure code and docs; not applied for the write-up

**[Read the case file →](https://khanhcloud.online/work/eks-terraform/)** · [Repository](https://github.com/iam-trongkhanh/EKS-Terraform)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Private S3 for build artifacts
<img alt="Amazon S3" src="https://img.shields.io/badge/Amazon_S3-252026?style=flat-square"> <img alt="IAM" src="https://img.shields.io/badge/IAM-252026?style=flat-square"> <img alt="AWS KMS" src="https://img.shields.io/badge/AWS_KMS-252026?style=flat-square"> <img alt="Terraform" src="https://img.shields.io/badge/Terraform-252026?style=flat-square&logo=terraform&logoColor=E5F481">

- Private bucket, ACLs disabled, versioning on
- CI role may upload only to the release prefix; requests without TLS denied
- SSE-KMS with a customer-managed key; S3 data events in CloudTrail
- Existing resources imported into Terraform until the plan showed no changes

**[Read the case file →](https://khanhcloud.online/work/secure-artifact-storage/)** · Completed personal lab

</td>
<td width="50%" valign="top">

### OrderFlow
<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-252026?style=flat-square&logo=typescript&logoColor=E5F481"> <img alt="Fastify" src="https://img.shields.io/badge/Fastify-252026?style=flat-square&logo=fastify&logoColor=E5F481"> <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-252026?style=flat-square&logo=postgresql&logoColor=E5F481"> <img alt="Docker" src="https://img.shields.io/badge/Docker-252026?style=flat-square&logo=docker&logoColor=E5F481">

- Order API with separate liveness (`/healthz`) and readiness (`/readyz`) checks
- Docker Compose stack, forward-only SQL migrations under an advisory lock
- Unit, integration (real PostgreSQL container) and Compose tests; Prometheus metrics
- Scope: local Docker Compose stack; AWS infrastructure in progress, no cloud resources provisioned yet

**[Repository →](https://github.com/iam-trongkhanh/orderflow-aws-devops)**

</td>
</tr>
</table>

## Toolbox.

**Cloud &amp; infrastructure** &nbsp;
<img alt="AWS" src="https://img.shields.io/badge/AWS-252026?style=flat-square"> <img alt="Terraform" src="https://img.shields.io/badge/Terraform-252026?style=flat-square&logo=terraform&logoColor=E5F481"> <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-252026?style=flat-square&logo=kubernetes&logoColor=E5F481"> <img alt="Docker" src="https://img.shields.io/badge/Docker-252026?style=flat-square&logo=docker&logoColor=E5F481">

**Delivery** &nbsp;
<img alt="Jenkins" src="https://img.shields.io/badge/Jenkins-252026?style=flat-square&logo=jenkins&logoColor=E5F481"> <img alt="Argo CD" src="https://img.shields.io/badge/Argo_CD-252026?style=flat-square&logo=argo&logoColor=E5F481"> <img alt="Git" src="https://img.shields.io/badge/Git-252026?style=flat-square&logo=git&logoColor=E5F481">

**Application** &nbsp;
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-252026?style=flat-square&logo=nodedotjs&logoColor=E5F481"> <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-252026?style=flat-square&logo=typescript&logoColor=E5F481"> <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-252026?style=flat-square&logo=postgresql&logoColor=E5F481"> <img alt="Next.js" src="https://img.shields.io/badge/Next.js-252026?style=flat-square&logo=nextdotjs&logoColor=E5F481">

## Activity.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/iam-trongkhanh/iam-trongkhanh/output/activity-dark.svg">
  <img alt="Contribution grid of iam-trongkhanh, drawn daily by a GitHub Actions workflow in this repository." src="https://raw.githubusercontent.com/iam-trongkhanh/iam-trongkhanh/output/activity-light.svg" width="100%">
</picture>

<sub>Generated daily by <a href=".github/workflows/activity.yml">a workflow in this repo</a>. Case files are written in English; each one ends with an evidence &amp; scope note.</sub>
