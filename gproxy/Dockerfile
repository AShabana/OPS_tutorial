FROM centos:7
MAINTAINER a.shabana@cequens.com 
RUN yum -y install  gcc git python-devel
RUN mkdir -p /app && echo "Creating app dir /app"
WORKDIR  /app
RUN curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"  && echo "Get the pip installer "
RUN python get-pip.py &&  echo "Install pip package manager .."
RUN git clone https://github.com/AShabana/gproxy gproxy
WORKDIR /app/gproxy
RUN pip install -r pip_requirement.txt
RUN pip install runtime
# Create config/app.conf
WORKDIR /app/gproxy/testing_tools
RUN ls
RUN python create_fake_firsttime_startup.py
WORKDIR /app/gproxy
