ssh-keygen
 
build -t lab2.v1 -f Dockerfile .

docker run -p 8080:8080 -d lab2.v1
 
docker tag lab2.v1 kazimierzdemucha/lab2.v1
 
docker push kazimierzdemucha/lab2.v1