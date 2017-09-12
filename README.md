# rainbow-sha256-go
Small webservice to return SHA256 Hashes and remember those to un-hash later.



#Docker      
docker-compose build      
docker-compose up      
      
 
#API      
**HASH** .   
http://0.0.0.0:9999/hash?str=ok .   
{"key":"ok","value":"2689367b205c16ce32ed4200942b8b8b1e262dfc70d9bc9fbc77c49699a4f1df"} .   

**REVERSE HASH** .   
http://0.0.0.0:9999/reverse_hash?str=2689367b205c16ce32ed4200942b8b8b1e262dfc70d9bc9fbc77c49699a4f1df .   
{"key":"2689367b205c16ce32ed4200942b8b8b1e262dfc70d9bc9fbc77c49699a4f1df","value":"ok"} .   

