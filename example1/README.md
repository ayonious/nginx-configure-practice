# Redirect http:localhost to https:localhost

## Step1: Generate an ssl certificate 
For simplicity lets generate a self signed ssl certificate.
```
cd example1
sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ayon.key -out ayon.crt
```


## Step2: Run the nginx
```
cd <path of nginx.conf file>
pwd 
# write the full path of the conf file
sudo nginx -c <full path of nginx.conf file>
```


## Step3: Test
Open browser and goto 127.0.0.1:6007, you will be redirected to whatever is running on 127.0.0.1:6006


## Step4: Stop nginx
```
sudo nginx -s stop
```

