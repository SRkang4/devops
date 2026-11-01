# Week09 Kubernetes

## 1. 클러스터 확인
minikube를 실행하고 kubectl get nodes 명령으로 Node가 Ready 상태임을 확인.

## 2. Deployment와 자가 치유
nginx Deployment를 replicas=3으로 생성함.
Pod 하나를 삭제하자 새로운 Pod가 자동으로 생성되어 다시 3개가 유지되는 것을 확인함.

## 3. Guestbook 배포
ghcr.io/srkang4/guestbook:v2 이미지를 Kubernetes Deployment로 실행함.
port-forward를 사용해 localhost:8080에서 방명록 화면을 확인함.

## 4. 오류 해결
처음에는 guestbook:v1 이미지가 존재하지 않아 ImagePullBackOff가 발생함.
이미지를 guestbook:v2로 변경하여 해결함.
