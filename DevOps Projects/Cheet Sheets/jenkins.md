 Jenkins
 --------------------------------

 
 - sudo systemctl stop jenkins
    - sudo systemctl start jenkins
    - sudo systemctl enable jenkins
    - sudo systemctl status jenkins
    - sudo journalctl -u jenkins -f -> live logs

- sudo netstat -tulnp | grep 8080 -> check port

 
 - name: Install dependencies
      run: npm install


    - name: Run tests
      npm run build
      run: npm test