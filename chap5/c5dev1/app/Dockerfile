FROM python:3.7.11-slim
LABEL author='myname@example.com'
RUN pip install Flask==1.1.1
COPY ./src/server.py /src/server.py
ENV PORT 80
CMD ["python", "-u", '/server.py']