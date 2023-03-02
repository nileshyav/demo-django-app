FROM python:3-alpine as builder
COPY . .    
RUN ["pip", "install", "-r", "requirement.txt"]
RUN ["python", "manage.py", "migrate"]
EXPOSE 8000
CMD ["python","manage.py","runserver","0.0.0.0:8000"]