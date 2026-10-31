

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,50:764ba2,100:f093fb&height=200&section=header&text=Shadahi%20Joseph&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Full-Stack%20Developer%20%7C%20AI%20Enthusiast%20%7C%20Designer&descAlignY=58&descColor=ffffffcc&animation=fadeIn" width="100%" />

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3500&pause=1000&color=a78bfa&center=true&vCenter=true&multiline=false&width=700&lines=Hey+there!+I'm+Joseph+%F0%9F%91%8B;3rd+Year+AI+%26+CS+Student+%40+KLU+University;Building+backends+with+Spring+Boot+%26+Java;Crafting+UIs+with+React.js+%26+Figma;Exploring+AI+Agents+%26+Intelligent+Systems)](https://git.io/typing-svg)

[![GitHub followers](https://img.shields.io/github/followers/Shadhai?style=for-the-badge&logo=github&color=764ba2&labelColor=1a1a2e)](https://github.com/Shadhai?tab=followers)
[![Profile Views](https://komarev.com/ghpvc/?username=Shadhai&color=764ba2&style=for-the-badge&label=PROFILE+VIEWS)](https://github.com/Shadhai)
[![Website](https://img.shields.io/badge/Portfolio-shadhai.github.io-667eea?style=for-the-badge&logo=googlechrome&logoColor=white)](https://shadhai.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shadhai-joseph-b7a746375/)

</div>
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4776e6,50:8e54e9,100:c471ed&height=200&section=header&text=Shadhai%20Joseph&fontSize=44&fontColor=ffffff&fontAlignY=38&desc=ML%20Researcher%20%7C%20Medical%20AI%20%7C%20Full-Stack%20Developer&descAlignY=58&descSize=17&animation=fadeIn" width="100%" />
</div>

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=A78BFA&center=true&vCenter=true&width=700&lines=Hey+there!+I'm+Joseph+%F0%9F%91%8B;3rd+Year+AI+%26+CS+Student+%40+KL+University;Medical+AI+%7C+GANs+%7C+Explainable+AI+%F0%9F%94%AC;Reproducible+ML+Research+over+leaderboard+chasing;Full-Stack+Engineer%3A+Spring+Boot+%26+React+%E2%9A%9B%EF%B8%8F" alt="Typing SVG" />
</div>

<div align="center">

[![GitHub followers](https://img.shields.io/github/followers/Shadhai?style=for-the-badge&logo=github&color=8e54e9&labelColor=1a1a2e)](https://github.com/Shadhai?tab=followers)
![Profile Views](https://komarev.com/ghpvc/?username=Shadhai&color=8e54e9&style=for-the-badge&label=PROFILE+VIEWS)
[![Portfolio](https://img.shields.io/badge/Portfolio-shadhai.github.io-4776e6?style=for-the-badge&logo=googlechrome&logoColor=white)](https://shadhai.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shadhai-joseph-b7a746375/)

</div>

---

## 👨‍💻 About Me

- 🔬 **Research focus:** Medical imaging, synthetic data reliability, and explainable deep learning
- 🔭 **Currently working on:** [A Controlled Augmentation Framework for GAN Quality in Medical AI](https://github.com/Shadhai/brain_tumor_gan_project) (technical report, under review)
- 🧠 **Core belief:** a metric going up is not the same as a model being right. I verify *why* something works
- 🏗️ **Also build:** production-style backends (Spring Boot, JWT, role-based APIs) and MERN full-stack apps
- 🌱 **Currently learning:** AI agents and intelligent systems
- 💬 **Ask me about:** GAN evaluation, class imbalance, Grad-CAM, Spring Boot, React
- ⚡ **Fun fact:** my GAN experiments run on a single RTX 3050, and I've learned that rigor matters more than raw compute

---

## 🔬 Research

### 🧪 A Controlled Augmentation Framework Reveals the Critical Role of GAN Quality

> A reproducibility-focused study on minority brain tumor detection in MRI

[![Repo](https://img.shields.io/badge/Repo-brain__tumor__gan__project-8e54e9?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Shadhai/brain_tumor_gan_project)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/Shadhai/brain_tumor_gan_project)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.1-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://github.com/Shadhai/brain_tumor_gan_project)
[![Stars](https://img.shields.io/github/stars/Shadhai/brain_tumor_gan_project?style=flat-square&color=yellow)](https://github.com/Shadhai/brain_tumor_gan_project/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/brain_tumor_gan_project?style=flat-square)](https://github.com/Shadhai/brain_tumor_gan_project)
![Status](https://img.shields.io/badge/Report-Under%20Review-orange?style=flat-square)

**The problem:** GANs are widely proposed to fix class imbalance in medical imaging, but most studies only check whether *classification improves* and never ask whether the synthetic images are *medically realistic*.

**The study:** The pituitary tumor class was cut to just **200 real MRI images** to simulate a rare condition. A class-specific **DCGAN** generated synthetic slices at increasing ratios, and an **EfficientNet-B0** classifier was trained on five datasets (D1 to D5) across **five random seeds**.

**The finding:** recall improved, but the GAN had not learned the real distribution.

| Evidence | Result | What it means |
|:---|:---|:---|
| Pituitary recall (val) | 0.880 → **0.984** with GAN data | Classification looks like a clear win |
| Pituitary recall (val), traditional aug | **0.994** | Simple augmentation matched or beat the GAN |
| FID, GAN sets | 231 to 235 | Very poor realism |
| FID, traditional aug | 113 | Better, but still imperfect |
| Real-vs-fake CNN | **99.8%** accuracy | Synthetic images are trivially separable |
| t-SNE | Disjoint clusters | No overlap with the real data manifold |

> **Takeaway:** performance improvement alone is *not* evidence of successful medical image generation. The repo proposes a reusable **multi-modal GAN verification protocol**: FID + real-vs-fake CNN + t-SNE + Grad-CAM + multi-seed statistics.

```mermaid
graph LR
    A[Brain MRI Dataset] --> B[Class-specific DCGAN]
    A --> C[Minority Scenario: 200 real images]
    B --> D[Synthetic MRI Slices]
    C --> E[D1 to D5 Datasets]
    D --> E
    E --> F[EfficientNet-B0 x 5 seeds]
    F --> G[Classification Metrics]
    D --> H[Quality Verification]
    H --> I[FID]
    H --> J[Real-vs-Fake CNN]
    H --> K[t-SNE]
    F --> L[Grad-CAM]
```

### 🧭 Research Interests

| Area | What I care about |
|:---|:---|
| 🧠 **Medical AI Safety** | Making sure models are trustworthy before they are accurate |
| 🎨 **Generative Models** | Evaluating whether synthetic data is actually realistic |
| 🔍 **Explainable AI** | Grad-CAM and attention validation against anatomy |
| ♻️ **Reproducibility** | Multi-seed statistics, open code, single-command pipelines |
| ⚖️ **Class Imbalance** | Rare-disease detection with limited real data |

---

## 🛠️ Tech Stack

<div align="center">

### 🤖 Machine Learning & Research
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![GANs](https://img.shields.io/badge/GANs-DCGAN-8e54e9?style=for-the-badge)
![EfficientNet](https://img.shields.io/badge/EfficientNet-B0-4776e6?style=for-the-badge)
![Grad-CAM](https://img.shields.io/badge/Explainable_AI-Grad--CAM-c471ed?style=for-the-badge)
![Computer Vision](https://img.shields.io/badge/Medical_Imaging-MRI-0f4c81?style=for-the-badge)
![AI Agents](https://img.shields.io/badge/AI_Agents-Exploring-412991?style=for-the-badge&logo=openai&logoColor=white)

### 💬 Languages
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### ⚛️ Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

### 🔧 Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)

### 🗄️ Database
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)

### 🧰 Tools & DevOps
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Shadhai&show_icons=true&theme=midnight-purple&include_all_commits=true&count_private=true&hide_border=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Shadhai&layout=compact&langs_count=8&theme=midnight-purple&hide_border=true"/>
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Shadhai&theme=midnight-purple&hide_border=true" />
</div>

---

## 📈 Contribution Activity

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Shadhai&theme=dracula&hide_border=true&area=true" width="100%" />
</div>

---

## 🏆 GitHub Trophies

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Shadhai&theme=onedark&no-frame=true&no-bg=true&row=1&column=7" />
</div>

---

## 🚀 Featured Projects

### 🧠 [Brain Tumor GAN Project](https://github.com/Shadhai/brain_tumor_gan_project) ⭐ *Flagship research*

> Controlled study of GAN-based augmentation for rare brain tumor detection, with a multi-modal verification protocol for synthetic medical images.

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/Shadhai/brain_tumor_gan_project)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://github.com/Shadhai/brain_tumor_gan_project)
[![Stars](https://img.shields.io/github/stars/Shadhai/brain_tumor_gan_project?style=flat-square&color=yellow)](https://github.com/Shadhai/brain_tumor_gan_project/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/brain_tumor_gan_project?style=flat-square)](https://github.com/Shadhai/brain_tumor_gan_project)

**What it does:** Trains a class-specific DCGAN on pituitary MRI slices, builds five controlled datasets (D1 to D5), and evaluates an EfficientNet-B0 classifier across five seeds. It then checks GAN realism with FID, a real-vs-fake CNN, t-SNE, and Grad-CAM, and shows that recall gains can occur even when the generator fails.  
**Tech used:** `Python` `PyTorch` `DCGAN` `EfficientNet-B0` `Grad-CAM` `FID` `t-SNE`

---

### 🚗 [Ultimate Car Rental Backend](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-)

> Enterprise-ready Spring Boot backend for a multi-role vehicle rental platform with secure authentication, payment processing, and analytics.

[![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-)
[![Stars](https://img.shields.io/github/stars/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-?style=flat-square&color=yellow)](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-/stargazers)
[![Forks](https://img.shields.io/github/forks/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-?style=flat-square&color=blue)](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-/network)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-?style=flat-square)](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-)

**What it does:** A vehicle rental management system with 4 roles (Admin, Local Head, Driver, Customer), each with scoped API access. Covers the full rental lifecycle from booking to driver payout, with JWT security, analytics dashboards, and Swagger docs.  
**Tech used:** `Java 17` `Spring Boot` `Spring Security` `JPA/Hibernate` `MySQL` `Swagger`

---

### 🍔 [Food Delivery App](https://github.com/Shadhai/fooddelivery)

> Full-stack MERN food delivery platform with user authentication, order tracking, and an admin dashboard.

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://github.com/Shadhai/fooddelivery)
[![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)](https://github.com/Shadhai/fooddelivery)
[![Stars](https://img.shields.io/github/stars/Shadhai/fooddelivery?style=flat-square&color=yellow)](https://github.com/Shadhai/fooddelivery/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/fooddelivery?style=flat-square)](https://github.com/Shadhai/fooddelivery)

**What it does:** A food ordering experience on the MERN stack: React + Vite frontend, Node.js/Express backend, MongoDB persistence. Supports menu browsing, cart management, and order placement.  
**Tech used:** `MongoDB` `Express.js` `React.js` `Node.js` `Vite`

---

### 🏷️ [Online Auction Platform](https://github.com/Shadhai/auction)

> A JavaScript auction platform with bid management, secure login, and auction scheduling.

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://github.com/Shadhai/auction)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://github.com/Shadhai/auction)
[![Stars](https://img.shields.io/github/stars/Shadhai/auction?style=flat-square&color=yellow)](https://github.com/Shadhai/auction/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/auction?style=flat-square)](https://github.com/Shadhai/auction)

**What it does:** Users create auctions, place bids, and track winning status. Built with plain JavaScript and CSS for a lightweight, dependency-free experience.  
**Tech used:** `JavaScript` `CSS3` `HTML5`

---

### ☕ [Spring Boot AC](https://github.com/Shadhai/springbootac)

> Spring Boot practice project exploring Java backend patterns, REST APIs, and enterprise architecture.

[![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://github.com/Shadhai/springbootac)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)](https://github.com/Shadhai/springbootac)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/springbootac?style=flat-square)](https://github.com/Shadhai/springbootac)

**What it does:** A sandbox for RESTful API patterns, JPA repositories, and Spring configuration, the proving ground behind the car rental system.  
**Tech used:** `Java` `Spring Boot` `Maven`

---

### ⚙️ [CI/CD Pipeline](https://github.com/Shadhai/ci-cd)

> Continuous Integration and Deployment experiments with automated workflows.

[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)](https://github.com/Shadhai/ci-cd)
[![Last Commit](https://img.shields.io/github/last-commit/Shadhai/ci-cd?style=flat-square)](https://github.com/Shadhai/ci-cd)

**What it does:** Explores CI/CD with GitHub Actions: automated build, test, and deployment workflows. This is the engineering discipline I bring to ML experiments too.  
**Tech used:** `GitHub Actions` `YAML` `DevOps`

---

## 📁 All Repositories

| Repository | Description | Domain | Language | Stars |
|:---|:---|:---|:---|:---:|
| [brain_tumor_gan_project](https://github.com/Shadhai/brain_tumor_gan_project) | GAN augmentation quality study for minority brain tumor detection | 🔬 ML Research | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) | ⭐ 1 |
| [Ultimate_Car_Rental_Backend-Spring-Boot-](https://github.com/Shadhai/Ultimate_Car_Rental_Backend-Spring-Boot-) | Enterprise Spring Boot backend for multi-role vehicle rental | 🔧 Backend | ![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) | ⭐ 3 |
| [fooddelivery](https://github.com/Shadhai/fooddelivery) | Full-stack MERN food delivery platform | 🌐 Full-Stack | ![JS](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | ⭐ 0 |
| [Food](https://github.com/Shadhai/Food) | Food-themed frontend UI project | ⚛️ Frontend | ![JS](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | ⭐ 0 |
| [auction](https://github.com/Shadhai/auction) | Online auction platform | 🌐 Full-Stack | ![JS](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | ⭐ 0 |
| [springbootac](https://github.com/Shadhai/springbootac) | Spring Boot REST API sandbox and practice repo | 🔧 Backend | ![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) | ⭐ 0 |
| [ci-cd](https://github.com/Shadhai/ci-cd) | GitHub Actions CI/CD pipeline experiments | ⚙️ DevOps | ![YAML](https://img.shields.io/badge/-YAML-CB171E?style=flat-square&logo=yaml&logoColor=white) | ⭐ 0 |
| [Shadhai](https://github.com/Shadhai/Shadhai) | 👤 Profile README repository | 📝 Meta | ![Markdown](https://img.shields.io/badge/-Markdown-000000?style=flat-square&logo=markdown&logoColor=white) | ⭐ 0 |

> 📦 **48 public repositories** in total. Explore them all at [github.com/Shadhai](https://github.com/Shadhai?tab=repositories)

---

## 🐍 Contribution Snake

<div align="center">
  <img src="https://raw.githubusercontent.com/Shadhai/Shadhai/output/github-contribution-grid-snake-dark.svg" alt="Snake animation" />
</div>

<!-- To enable the snake: follow https://github.com/Platane/snk to set up the GitHub Action -->

---

## 🤝 Connect With Me

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Shadhai)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shadhai-joseph-b7a746375/)
[![Portfolio](https://img.shields.io/badge/Portfolio-8e54e9?style=for-the-badge&logo=googlechrome&logoColor=white)](https://shadhai.github.io/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:2300032260@kluniversity.in)

<br/>

> 💡 *"Reproducibility is not optional in medical AI."*

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:c471ed,50:8e54e9,100:4776e6&height=120&section=footer" width="100%" />

</div>
