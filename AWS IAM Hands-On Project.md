# 🚀 AWS IAM Hands-On Project

This hands-on project demonstrates the use of **AWS Identity and Access Management (IAM)** to create and manage users, groups, roles, and policies.

🔐 IAM is a core security service in AWS, and mastering it is essential for cloud engineers, DevOps, and security professionals.

> 🧠 **This was my first-ever recorded tutorial. Kindly bear with any rough edges. I’m learning and promise to get better.** 🙏

---

## 📹 Watch the Video

🎥 [Watch it on LinkedIn](#)  
📂 [Project Files on GitHub](https://github.com/Edimulo1)

---

## 🛠️ What This Project Covers

- ✅ Creating an IAM User (`dev-user`)
- ✅ Creating an IAM Group (`DevTeam`) and attaching permissions
- ✅ Assigning Users to Groups
- ✅ Creating a Role for EC2 to Access S3 (`EC2S3AccessRole`)
- ✅ Writing and Attaching a Custom IAM Policy for `s3:GetObject`

---

## 📂 File Descriptions

| File | Description |
|------|-------------|
| `README.md` | Main overview of the project |
| `iam-steps.md` | Step-by-step guide for reproducing the project |
| `custom-policy.json` | Sample JSON file for the custom IAM policy |
| `screenshots/` | Folder containing screenshots of each step |

---

## 📘 How to Use This Repo

1. Clone or download this repository.
2. Follow `iam-steps.md` to recreate the setup in your own AWS Console.
3. Replace the bucket name in `custom-policy.json` with your actual S3 bucket name.
4. Use screenshots for reference or documentation.

---

## 🔐 Sample Custom Policy

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
