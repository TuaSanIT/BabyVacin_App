# Baby Vacin
Baby Vaccination Tracker

##Hướng dẫn cài đặt dự án Baby Vaccination Tracker

#Dự án bao gồm 3 ứng dụng : UserApp, VaccineCenterApp, AdminApp
và 1 Backend

#Cài đặt Backend
1. Cài môi trường NodeJS 
	https://nodejs.org/en

2.Thiết lập tài nguyên
root
	-.env: điền OpenAI Key
	-app
	|
	--controllers
		|
		--ChatController.js : Điền Assistant Key
3. Tạo terminal chạy lần lượt:
	$	npm i
	$	npm start

#Cài đặt Ứng dụng:
1. Cài đặt môi trường Java Development Kit
	https://www.oracle.com/java/technologies/downloads

2. Cài đặt Android Studio:
	https://developer.android.com/studio

3. Setup Project:
	3.1 Vào Android Studio mở Thư mục dự án 
	3.2 Sync Gradle 
	3.3 Vào Tools -> Firebase -> Firebase Realtime,  Firebase Authencation
	3.4 Thiết lập client (UserApp): ..\app\src\main\java\com\prox\babyvaccinationtracker\RetrofitClient.java
		.baseUrl("http://192.168.1.5:3000/") 
		-> .baseUrl("http://<ip.address.v4>:3000/")
	3.5 Build Project
