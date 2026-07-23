# CyberLab(picoCTF) Writeup [Old Sessions]

## 📝 Challenge Information
* **Category:** Web Exploitation
* **Points:** [100]
* **Difficulty:** [Easy ]
* **Tags:** #web #cookies

## 🎯 Objective
Find the hidden flag.

## Solution Steps
1. **Step 1:** Open the target URL and navigate to the login page.You shoul seeing this:
 <img width="745" height="476" alt="image" src="https://github.com/user-attachments/assets/978519b4-cbd8-4231-8e46-ef89db9c70e3" />

2. **Step 2:** You have to login. for example I use
   ```
   username: b
   password: b
4. **Step 3:** Once you are logged, you have to see this:
   <img width="812" height="637" alt="image" src="https://github.com/user-attachments/assets/c3c5c585-5722-4861-9761-e9d87c66af25" /> 
4. **Step 4:** Now the logicall thing is you are b and you have to move to admin, but how you do that?, well first we go to that directoty(hint) that the lab gave to us. And we see this:
   <img width="943" height="321" alt="image" src="https://github.com/user-attachments/assets/e694461c-69b1-421c-aac8-5f6b76768900" />

   We can see to logs of loggin sesions ours and the admin. and that chain of characters looks like a cookie so, we can try to use that cookie and see if makes us admin
  5. **Step 5:** Using
     <img width="946" height="703" alt="image" src="https://github.com/user-attachments/assets/c381ad67-0690-47be-906a-101d4eb5ebd6" />
 

## 🏁 Flag


```flag
picoCTF{y0ur_fl4g_h3r3}

```

## 💡 Key Takeaways & Mitigation
* **What I learned:** [e.g., Always sanitize user input before passing it to SQL queries.]
* **Remediation:** Implement prepared statements and parameterized queries to prevent this flaw.
