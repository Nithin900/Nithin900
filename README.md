# Hi, I'm Nithin 👋

**Java backend developer** · Spring Boot · Spring Security · Microservices
📍 Greater Toronto Area · Open to Java backend and application support roles

I build secure, well-tested Spring services and like understanding *why* the framework behaves the way it does, from the filter chain down to the bean lifecycle.

---

## 🔐 Featured project: [SecurePay — Payment Security Journey](https://github.com/Nithin900/PaymentSecurityJourney)

A payment system split into four Spring Boot services, secured end to end with OAuth 2.0 and JWT.

```
Client ──login──► Auth Server :9000 ──JWT──► Client
Client ──Bearer JWT──► Gateway (A) :8080 ──token relay──► Payment (B) :8081 ──► DB
                                                   │ client_credentials JWT
                                                   ▼
                                     Notification :8082 ──► SMTP
```

- **Spring Authorization Server** issues RS256-signed JWTs (authorization code + client credentials flows)
- **Scope-based access** per HTTP method; **ownership enforced** from the token's `sub` (other users get 404)
- **Zero-trust between services** — B re-validates every token instead of trusting the gateway
- **Resilience** — WebClient timeouts, 503 when downstream is unreachable, email failure never fails a payment
- **Consistent error contract** (400 / 404 / 409 / 502 / 503) via `GlobalExceptionHandler`
- **25+ automated end-to-end checks** plus unit tests with `@MockitoBean`

`Java 17` `Spring Boot 3.5` `Spring Security 6.5` `Spring Authorization Server` `JPA / H2` `WebClient` `Maven` `GitHub Actions`

🌐 [Interactive explainer site](https://nithin900.github.io/PaymentSecurityJourney/) — a request traced hop by hop through the real code

---

## 🧩 Also worth a look

| Project | What it shows |
|---|---|
| [Spring Core Fundamentals](https://github.com/Nithin900/Fundementals-spring-core) | DI (XML / Java / annotations), bean scopes and lifecycle, and an AOP module with custom aspects for timing, security, audit, retry and per-invocation trace IDs |
| [Health Care Price Tool](https://github.com/Nithin900/Health-Care-Price-Tool) | Python + Flask app serving a scikit-learn insurance price model |

---

## 🛠 Tech

**Backend:** Java (8–21) · Spring Boot · Spring Security · OAuth 2.0 / JWT · JPA / Hibernate · REST · Kafka
**Data:** Oracle · MySQL · SQL Server · H2
**Ops & debugging:** OpenShift · Kibana · JVM thread dumps · Maven · Git · GitHub Actions
**Also:** Python · Pandas · scikit-learn · Tableau · Power BI

---

## 📫 Reach me

[LinkedIn](https://www.linkedin.com/in/nithinarumbakam)
# Nithin Arumbakam

📧 **Email:** nitin.arumbakam@gmail.com  
📞 **Phone:** +1 437 441 8928  
📍 **Location:** Windsor, ON, N9C 1W5  
🔗 [**LinkedIn**](www.linkedin.com/in/nithinarumbakam)
---

## 🛠 Skills

- **Programming Languages:** Python, SQL, Excel  
- **Data Analysis Libraries:** NumPy, Pandas, Matplotlib, Seaborn   
- **Machine Learning:** Scikit-Learn, TensorFlow, Keras  
- **Database Management:** MySQL, SQL Server  
- **Data Visualization Tools:** Tableau, Power BI  
- **Version Control:** Git, GitHub  
- **Soft Skills:**  
  - Excellent verbal and written communication for presenting technical information  
  - Effective time management in fast-paced environments  
  - Proven team collaboration and independent work capabilities  

---

## 🎓 Education

**Post Graduate Diploma in Management: Data Analytics for Business**  
**St. Clair College, Windsor, ON** | *January 2024 – Present*  
- **Availability:** 4-8 months Co-op/internship starting May 2025  
- **Relevant Coursework:**  
  - Data Analysis and Visualization  
  - Statistical Analysis  
  - Business Intelligence  
  - Machine Learning for Business  
  - Database Management Systems  
  - AWS  
  - Project Management Analytics  

---

## 📂 Academic Projects

### **Health Care Price Tool & Insurance Price Prediction Model**  
*St. Clair College, ON, Canada | October 2024 – December 2024*  
- **Problem:** Difficulty in selecting cost-effective insurance plans due to varying user needs, medical history, and budget constraints.  
- **Solution:**  
  - Designed and implemented a healthcare price tool with a machine learning model using Scikit-learn, achieving 15% predictive accuracy.  
  - Integrated the model into a Flask-based web application.  
  - Performed data preprocessing, feature engineering, and hyperparameter tuning to enhance performance.  
  - Created visualizations using Matplotlib for cost breakdowns and plan comparisons, improving user decision-making.

### **Graduate Employment Statistics Analysis**  
*St. Clair College, ON, Canada | January 2024 – April 2024*  
- **Objective:** Analyze graduate employment trends across Canada to understand the impact of education level, field of study, gender, and region on employment outcomes.  
- **Key Activities:**  
  - Explored variations in median employment income based on education qualification and geographic region.  
  - Performed statistical analysis on gender and age group employment trends.  
  - Developed interactive visualizations using Python (Matplotlib, Seaborn) and Tableau to represent employment data from 2010–2014.  
- **Outcome:** Identified actionable insights for improving graduate employability, enabling data-driven policy decisions.

### **Customer Churn Prediction and Analysis**  
*St. Clair College, ON, Canada | October 2024 – December 2024*  
- **Problem:** High customer churn rates affecting revenue and retention strategies.  
- **Solution:**  
  - Implemented a Python-based churn prediction model using historical customer data.  
  - Utilized machine learning algorithms and feature engineering to improve churn prediction accuracy by 15%.  
  - Visualized insights with Tableau, aiding decision-making and reducing churn rates by over 20% through targeted retention initiatives.  



---

## 💼 Experience

### **Systems Engineer**  
**Infosys Consulting Services, Chennai, India** | *July 2022 – August 2023*  
- Developed and maintained software applications according to client specifications.  
- Provided technical support and troubleshooting for software issues.  
- Collaborated with cross-functional teams to ensure seamless project delivery.  
- Conducted system testing and validation to ensure optimal performance.  
- Created and maintained documentation for software applications and processes.
