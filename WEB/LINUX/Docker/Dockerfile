# escape=`
                
FROM dmdock247/repo:mill-nginx
                

## location of the source directory & also copy the directory "nginx-content" here which includes index.html
WORKDIR /etc/nginx/conf.d/
COPY nginx-content/ /usr/share/nginx/html/

                
## Check that the files have been successfully copied
RUN cat /usr/share/nginx/html/index.html

