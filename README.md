## ClaylDy_HF_Demo
A VR game account management system which user can log in via RFID.

### How to use this project?
- Step 1. Prepare a ClayIDy USBto read RFID
- Step 2. Install __.exe__ of ClayIDy
- Step 3. Change the correct path of project file in **MyPage.cs** <br/>
  ```
  [64] pictUser.Image = System.Drawing.Image.FromFile("C:\\Users\\User\\Downloads\\ClarIDy_HF_Demo A.4\\Photo\\男-removebg-preview.png");
  [66] pictUser.Image = System.Drawing.Image.FromFile("C:\\Users\\User\\Downloads\\ClarIDy_HF_Demo A.4\\Photo\\女-removebg-preview.png");
  [100] StreamWriter sw = new StreamWriter(@"C:\Users\User\Downloads\ClarIDy_HF_Demo A.4\UserInfo.txt");
  ```
- Step 4. The button of __`進入遊戲`__ in MyPage is for open a file when user tap it, so you can change to any file you would like to open when tap it. <br/>
  ```
  [108] Process.Start(@"D:\GoodProject\GoodProject.uproject");
  ```
  
### All of Page in this project
* **Top Page**: Sign up page, user can sign up and bind ID card in this page.
* **Login by card Page**: When user tap **`已有帳號?`** button, it would open this form, then user can put ID card on ClayIDy to login.
* **Login by account Page**: When user tap **`以學生證登入`** button, it would open this form, then user can fill this form to login.
* **My Page**: When user login successfully, it would open this form. And it would show user information.
* **Intro Page**: When user tap **`遊戲介紹`** button, it would show this page to introduce VR game.
