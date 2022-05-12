# GitOps
 
CI job에서 이미지를 빌드하고 컨테이너 레지스트리(ECR)에 푸시하면,
CD job에서 kustomize를 사용하여 최신 이미지 태그로 오버레이 하고, 다시 Github repository에 변경 내용을 푸시합니다.

<br>

이후 이 리포지토리와 연결된 Argo CD가 변경된 최신 이미지 태그로 쿠버네티스와의 싱크를 맞춰줍니다.

<br>
