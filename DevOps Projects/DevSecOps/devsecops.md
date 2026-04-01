# 🔐 DevSecOps Interview Questions & Answers

---

# 🔹 DEVSECOPS BASICS

## 1. What is DevSecOps?
DevSecOps means integrating security into DevOps pipeline.

👉 Security is included at every stage.

---

## 2. Why DevSecOps?
- Early vulnerability detection
- Secure applications
- Automation

---

## 3. What is shift-left security?
Testing security early in development.

---

## 4. What are types of security testing?
- SAST (Static)
- DAST (Dynamic)
- SCA (Dependency scan)

---

## 5. What is vulnerability?
Weakness in system that can be exploited.

---

# 🔹 SONARQUBE

## 6. What is SonarQube?
Tool for code quality and security analysis.

---

## 7. What type of testing?
SAST (Static Analysis)

---

## 8. What does SonarQube check?
- Code bugs
- Vulnerabilities
- Code smells

---

## 9. What is Quality Gate?
Rules to pass code quality.

---

## 10. What is code smell?
Bad coding practice.

---

## 11. What is coverage?
Percentage of code tested.

---

## 12. SonarQube in CI/CD?
Runs during build stage.

---

## 13. What happens if Quality Gate fails?
Pipeline fails.

---

## 14. What is Sonar Scanner?
Tool to scan code.

---

## 15. What languages supported?
Java, Python, JS, etc.

---

# 🔹 TRIVY

## 16. What is Trivy?
Security scanner for containers and code.

---

## 17. What does Trivy scan?
- Docker images
- File system
- Kubernetes

---

## 18. What type of scan?
SCA + vulnerability scanning

---

## 19. How to use Trivy?
trivy image nginx

---

## 20. What does Trivy detect?
- CVEs
- Misconfigurations
- Secrets

---

## 21. Trivy in CI/CD?
Scan images before deployment.

---

## 22. Why scan containers?
To avoid vulnerable images.

---

## 23. What is CVE?
Common Vulnerabilities and Exposures.

---

## 24. What is severity level?
Low, Medium, High, Critical

---

## 25. How to fix vulnerabilities?
Update packages or base image.

---

# 🔹 OWASP

## 26. What is OWASP?
Open Web Application Security Project.

---

## 27. What is OWASP Top 10?
List of top security risks.

---

## 28. Examples?
- SQL Injection
- XSS
- Broken Authentication

---

## 29. What is SQL Injection?
Inject malicious SQL queries.

---

## 30. What is XSS?
Inject scripts into web pages.

---

## 31. What is CSRF?
Unauthorized actions using user session.

---

## 32. How to prevent OWASP risks?
- Input validation
- Authentication
- Encryption

---

## 33. What is dependency check?
Scan libraries for vulnerabilities.

---

## 34. OWASP in DevOps?
Used in security testing phase.

---

## 35. Tools related to OWASP?
- ZAP
- Dependency Check

---

# 🔹 PROMETHEUS

## 36. What is Prometheus?
Monitoring and alerting tool.

---

## 37. How it works?
Pulls metrics from targets.

---

## 38. What is metric?
Data about system (CPU, memory).

---

## 39. What is exporter?
Tool to expose metrics.

---

## 40. What is PromQL?
Query language for metrics.

---

## 41. What is alert manager?
Handles alerts.

---

## 42. Prometheus in Kubernetes?
Used for cluster monitoring.

---

## 43. What is scraping?
Collecting metrics.

---

## 44. Data storage?
Time-series database.

---

## 45. Example metrics?
CPU usage, memory usage

---

# 🔹 GRAFANA

## 46. What is Grafana?
Visualization tool for monitoring data.

---

## 47. What does Grafana do?
Creates dashboards.

---

## 48. What data sources?
Prometheus, Elasticsearch, etc.

---

## 49. What is dashboard?
Visual representation of metrics.

---

## 50. What is panel?
Single graph in dashboard.

---

## 51. Grafana alerts?
Trigger alerts based on metrics.

---

## 52. Why use Grafana?
Better visualization.

---

## 53. Grafana with Prometheus?
Prometheus collects → Grafana displays.

---

## 54. What is templating?
Dynamic dashboards.

---

## 55. What is alerting?
Notify when thresholds crossed.

---

# 🧪 REAL-TIME SCENARIOS

## 56. Vulnerability found in image?
- Fix Dockerfile
- Update base image
- Re-scan

---

## 57. Code quality failed?
Fix issues in SonarQube.

---

## 58. High CPU alert?
Check Prometheus metrics.

---

## 59. Dashboard not showing data?
Check data source.

---

## 60. Security issue in production?
- Identify vulnerability
- Patch immediately
- Redeploy

---
