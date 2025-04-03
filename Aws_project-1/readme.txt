# 🌐 AWS Static Website Hosting with S3, CloudFront, Route 53 & ACM

This project demonstrates how to host a static website on AWS using:
- **Amazon S3** (Stores website files)
- **AWS CloudFront** (Content Delivery Network)
- **Route 53** (DNS Configuration)
- **AWS ACM** (SSL Certificate for HTTPS)

---

## 🚀 Step-by-Step Guide

### 1️⃣ Register a Domain  
- Purchased domain from **GoDaddy** (`tirueplantshoppingcart.shop`).

### 2️⃣ Create an S3 Bucket  
- Bucket Name: **`my-website-bucket`**  
- Disabled Public Access (CloudFront will serve content)  
- Uploaded website files (`index.html`, `styles.css`, etc.)

### 3️⃣ Set Up CloudFront  
- Origin: **S3 Bucket**
- Enabled **HTTPS**
- Configured **Alternate Domain Names (CNAMEs)**

### 4️⃣ Configure Route 53  
- **A Record (Alias)** → Points to **CloudFront Distribution**  
- **CNAME Record (Optional)** → `www.tirueplantshoppingcart.shop` → `tirueplantshoppingcart.shop`

### 5️⃣ SSL Certificate (AWS ACM)  
- Issued a **free SSL certificate** via **AWS Certificate Manager (ACM)**  
- Validated using **Route 53 CNAME record**

---

## 🔍 Testing  
- **Domain Name**: [https://tirueplantshoppingcart.shop](https://tirueplantshoppingcart.shop)  
- **DNS Verification**: [https://www.whatsmydns.net](https://www.whatsmydns.net)

---

## 📸 Screenshots  
- ✅ **S3 Bucket Settings**  
- ✅ **CloudFront Distribution**  
- ✅ **Route 53 DNS Records**  
- ✅ **ACM SSL Certificate**  

---

## 📝 Notes  
- 🔒 **Why CloudFront?** Security + Performance  
- 🌍 **DNS Propagation:** May take **5-30 minutes**  
- 🛠 **Troubleshooting:** Check CloudFront logs if errors occur  

---

## 🤝 Contributing  
Feel free to fork, star ⭐, or submit improvements!

---

## 📜 License  
MIT License © 2025 Ragi Sai Bhavani
