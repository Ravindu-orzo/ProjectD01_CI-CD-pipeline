# ProjectD01_CI-CD-pipeline
Goal here is to implement a real DevSecOps pipeline. Research needs to be done first to understand what gates are used in CI/CD pipelines then they will be implemented.

### Link to Team Repo : https://github.com/Ravindu-orzo/NodeGoat

### Part I was reponsible for making: DevSecOps pipeline

- It has 5 security gates
1. SAST Scan - using both CodeQL and semgrep.
2. Dependancy scan - using NPM Audit
3. Container image scan - using Trivy
4. Secret scan - using GitLeaks
5. DAST Scan - using OWASP ZAP

- Only the secret scan is configured to fail the pipeline. This design choice was taken as per the requirements of the project. However in real production all gates should be configured to fail.
- Other gates are configured to WARN only.
