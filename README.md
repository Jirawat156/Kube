# Kube
## การติดตั้ง kubectl
ทำการโหลด kubectl
- https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/
![image](https://user-images.githubusercontent.com/119155285/226195637-26679ade-1e1e-430f-8a19-073ad0b94034.png)
เข้าไปสร้างที่ไดฟ์ C ตั้งชื่อ kubectl แล้วนำไฟล์ที่โหลดมาเข้าไปไว้ที่โฟลเดอร์<br>
![image](https://user-images.githubusercontent.com/119155285/226195688-37f6e803-b95f-4b11-9ab1-2719646137c6.png)
![image](https://user-images.githubusercontent.com/119155285/226195701-d0d5dbc2-d4fe-47a4-b39b-d6b6486b306c.png) <br>
นำ Path ไปเพิ่มใน environment <br>
![image](https://user-images.githubusercontent.com/119155285/226195819-8b631ff6-393b-4111-9eef-d00dd03e593d.png)

## การติดตั้ง minikube
ทำการโหลด minikube
- https://minikube.sigs.k8s.io/docs/start/
![image](https://user-images.githubusercontent.com/119155285/226196026-ef32b655-455a-4dcd-bafd-fb6cf6d5b447.png)
ทำการติดตั้ง minikube จากนั้นตัว minikube จะสร้างpathในenvironmentให้<br>
![image](https://user-images.githubusercontent.com/119155285/226196105-8e57ab0e-f11a-4b14-8239-af8005602cc3.png)

## การติดตั้ง Docker Desktop for Windows
ทำการโหลด Docker Desktop for Windows
- https://docs.docker.com/desktop/install/windows-install/
![image](https://user-images.githubusercontent.com/119155285/226196293-ad7fcbb4-843a-43a7-b2a3-7dbb0e927808.png)

สิ่งที่ได้จากการติดตั้ง Docker Desktop for Windows
![image](https://user-images.githubusercontent.com/119155285/226196361-e9e5d5b7-6fc9-41ac-b526-a1c3ebc3d329.png)

## การ deploy Traefik
Ref : https://github.com/iamapinan/kubeplay-traefik

ทำการเพิ่ม 127.0.0.1 traefik.spcn24.local ในไฟล์ hosts <br>
ที่ path C:\Windows\System32\drivers\etc
![image](https://user-images.githubusercontent.com/119155285/226196503-3324118a-5ce2-4db7-a728-b564ab137443.png)
- ติดตั้ง Install Traefik โดยใช้คำสั่งนี้
   
       kubectl apply -f https://raw.githubusercontent.com/traefik/traefik/v2.9/docs/content/reference/dynamic-configuration/kubernetes-crd-definition-v1.yml
