# 🚀 CI/CD Interview Questions & Answers

---
  🔹What is DevOps?

***Answer:***

DevOps is a way of working where developers and operations teams collaborate to build, test, and release software faster and more reliably.

👉 Goal: Faster delivery + fewer errors

## 1. What is CI/CD?
CI/CD is a process to automate software delivery.

- CI = Continuous Integration (Automatically testing code when developers push changes)
- CD = Continuous Delivery/Deployment (Automatically releasing code to production)

---

## 2. What is Continuous Integration (CI)?
CI means developers merge code frequently and run automated tests.

👉 Goal: Detect bugs early

---

## 3. What is Continuous Delivery?
Code is always ready to deploy, but requires manual approval.

---

## 4. What is Continuous Deployment?
Code is automatically deployed to production without manual steps.

---

## 5. What is a CI/CD pipeline?
A pipeline is a sequence of automated steps:

Code → Build → Test → Deploy

---

## 6. Why use CI/CD?
- Faster releases
- Fewer bugs
- Automation
- Better collaboration

---

## 7. What are common CI/CD tools?
- Jenkins
- GitHub Actions
- GitLab CI
- Azure DevOps

---

## 8. What is a build?
Converting source code into a runnable application.

---

## 9. What is automated testing?
Running tests automatically to validate code.

---

## 10. What is a pipeline stage?
Each step in pipeline (build, test, deploy).

---

# 🔹 INTERMEDIATE QUESTIONS

## 11. What triggers a CI/CD pipeline?
- Code push
- Pull request
- Scheduled jobs

---

## 12. What is a rollback?
Reverting to a previous working version.

---

## 13. What is artifact?
A built file (e.g., .jar, .zip, Docker image).

---

## 14. What is pipeline failure?
When any stage fails (build/test/deploy).

---

## 15. What is version control in CI/CD?
Tracking changes using Git.

---

## 16. What is branching strategy?
Ways to manage code branches (Git Flow, trunk-based).

---

## 17. What is environment in CI/CD?
Different stages:
- Dev
- Staging
- Production(Prod)

---

## 18. What is YAML in CI/CD?
Configuration file format for pipelines.

---

## 19. What is secret management?
Secure storage of passwords, API keys.

---

## 20. What is parallel execution?
Running multiple jobs at same time to save time.

---

# 🔹 ADVANCED CI/CD QUESTIONS

## 21. What is Blue-Green Deployment?
Two environments:
- Blue = current
- Green = new

Switch traffic when ready.

---

## 22. What is Canary Deployment?
Release to small users first, then gradually increase.

---

## 23. What is Infrastructure as Code in CI/CD?
Managing infrastructure using code (Terraform).

---

## 24. What is containerization in CI/CD?
Using Docker to package apps for consistent deployment.

---

## 25. What is orchestration?
Managing containers using Kubernetes.

---

## 26. What is pipeline as code?
Defining pipelines in code (YAML).

---

## 27. What is caching in CI/CD?
Saving dependencies to speed up builds.

---

## 28. What is zero downtime deployment?
Deploying without affecting users.

---

## 29. What is test coverage?
Percentage of code tested.

---

## 30. What is shift-left testing?
Testing early in development.

---

# 🧪 HANDS-ON SCENARIO QUESTIONS

## 31. What happens when you push code?
1. Code pushed to Git
2. Pipeline triggers
3. Build runs
4. Tests run
5. Deploy if success

---

## 32. Pipeline failed, what will you do?
- Check logs
- Identify error
- Fix issue
- Re-run pipeline

---

## 33. How do you deploy safely?
- Use staging
- Use blue-green or canary
- Monitor logs

---

## 34. How do you handle secrets?
- Use secret managers
- Avoid hardcoding

---

## 35. How do you improve pipeline speed?
- Use caching
- Parallel jobs
- Optimize tests

---

## 36. How do you debug deployment issues?
- Check logs
- Check configs
- Verify environment

---

## 37. How do you rollback deployment?
- Re-deploy previous version
- Use version tags

---

## 38. What if tests fail?
- Stop deployment
- Fix bugs
- Re-run pipeline

---

## 39. How do you ensure quality?
- Automated tests
- Code reviews
- Monitoring

---

## 40. What is your CI/CD workflow?
Code → Git → CI → Test → Build → Deploy → Monitor

---

# ☁️ AWS CI/CD QUESTIONS

## 41. What AWS services are used in CI/CD?
- CodeCommit (Git)
- CodeBuild (build)
- CodeDeploy (deploy)
- CodePipeline (pipeline)

---

## 42. What is AWS CodePipeline?
Service to automate CI/CD workflow.

---

## 43. What is AWS CodeBuild?
Build and test code in AWS.

---

## 44. What is AWS CodeDeploy?
Deploy applications to servers.

---

## 45. What is artifact in AWS?
Output stored in S3.

---

## 46. What is IAM role in CI/CD?
Permissions for services to interact.

---

## 47. How do you secure AWS pipelines?
- IAM roles
- Encryption
- Secrets Manager

---

## 48. What is S3 role in CI/CD?
Store artifacts and pipeline data.

---

## 49. What is CloudWatch in CI/CD?
Monitoring and logs.

---

## 50. How do you deploy using AWS CI/CD?
CodeCommit → CodeBuild → CodeDeploy → Production

---

