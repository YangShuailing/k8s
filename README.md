# k8s
1. 测试
git clone https://github.com/googlecontainers/kubernetes-dashboard-ppc64le.git
touch Dockerfile，内容如下
FROM gcr.io/google_containers/kubernetes-dashboard-ppc64le:v1.8.0
git commit -m ‘v1.8.0’
git tag v1.8.0
修改Dockerfile内容如下
FROM gcr.io/google_containers/kubernetes-dashboard-ppc64le:v1.8.1
git commit -m ‘v1.8.1’
git tag v1.8.1
修改Dockerfile内容如下
FROM gcr.io/google_containers/kubernetes-dashboard-ppc64le:v1.8.2
git commit -m ‘v1.8.2’
git tag v1.8.2
git push --tags



FROM k8s.gcr.io/kube-cross:v1.11.5-1
