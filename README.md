## Ynet News And Bitcoin Price With kubernetes 


Kubernetes project that shows price of BitCoin and displays the latest news from Ynet:

● Presents the Current BitCoin Price, And the Average Price for the last 10 minutes and stores the price in a Redis Database.

● Reads the “Breaking News” from YNet news service.


## Run With Minikube:
```bash
 git clone https://github.com/saeedismael/kubernetesTask.git

 cd YnetNews_bitcoinPrice_kubernetes

 minikube start

 minikube addons enable ingress

 kubectl apply -f .

 minikube tunnel
```

## Access from browser:
http://localhost/bitcoin

http://localhost/ynet

## Run the apps with Docker
 docker pull cyberpunks77/bitcoin-price

 docker run -d -p 8000:5000 cyberpunks77/bitcoin-price
 
 ![bitcoin](https://user-images.githubusercontent.com/49121054/181013115-7ab0fb0f-181e-4458-a0dc-333d533867cf.jpg)



 docker pull cyberpunks77/ynet

 docker run -d -p 8000:5000 cyberpunks77/ynet
 ![bitcoin](https://user-images.githubusercontent.com/49121054/181013142-ccf8b37e-c03b-4f27-9b4d-2418d83c71bb.jpg)

 
