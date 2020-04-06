# Version： 0.0.1

FROM centos:latest
MAINTAINER Qiuye "qiuye.wz@gmail.com"
RUN yum install -y wget
RUN mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo_bak
RUN wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-8.repo
RUN yum install -y nginx
RUN echo "Hi, I am in your container" >/usr/share/nginx/html/index.html
EXPOSE 80

ENTRYPOINT ["/usr/sbin/nginx"]
CMD ["-h"]