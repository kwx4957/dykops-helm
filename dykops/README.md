# dykOps helm Repository

### How to use
1. helm lint .
2. helm template .
3. helm install dykops . --debug --dry-run
4. helm pacagke .

해당 과정을 수행하면 .tgz 파일이 생성된다. 생성된 .tgz 파일은 /stable 디렉토리에 위치시킨다. 
index.yaml에 해당 내용을 반영한다.  

5. helm repo index . 
6. git add & commit & push

helm 저장소를 최신화하기 위해서 다음 명령어를 수행한다.  
6. helm repo update

### 저장소 추가하기
1. helm repo add {my-helm-repo} https://kwx4957.github.io/dykops-helm/stable/
2. helm install dykops dykops/dykops -n helmtest 

실행된 버전 종료 
3. helm uninstall dykops

