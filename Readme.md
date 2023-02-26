ZAP 
  docker run -v $(pwd):/zap/wrk/:rw -t owasp/zap2docker-stable zap-baseline.py \ -t https://www.example.com -g gen.conf -r testreport.html
  https://www.zaproxy.org/docs/docker/baseline-scan/
  
  docker run -t owasp/zap2docker-stable zap-api-scan.py -t https://api.net/swagger/v1/swagger.json -f openapi
  
  https://www.zaproxy.org/docs/docker/
  
Nikto
 docker run --rm -v C:\temp:/tmp sullo/nikto -h https://app.net -o /tmp/out.json
