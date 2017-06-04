# Redirect http:localhost to https:localhost

## Step1: Generate an ssl certificate (for simplicity lets generate a self signed ssl certificate)
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
```

```

## Step4: Stop nginx
```

```
