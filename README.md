@ privé master: 172.31.39.227
@publich master: 3.144.140.151
@Public IPv4 DNS: ec2-3-144-140-151.us-east-2.compute.amazonaws.com
zone: us-east-2
Partie1:
1)exposition de service de l'application kubeadm 
           http://3.144.140.151:30268

2)dashboard kubernetes: 
           https://52.15.239.38:30878/#/overview?namespace=default s
token : 
eyJhbGciOiJSUzI1NiIsImtpZCI6IjFOTEI2cTFqUlF3MzRONmZWdmVWaVBRRlZwenNReGdFT251QXYzM2xJd00ifQ.eyJpc3MiOiJrdWJlcm5ldGVzL3NlcnZpY2VhY2NvdW50Iiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9uYW1lc3BhY2UiOiJrdWJlcm5ldGVzLWRhc2hib2FyZCIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VjcmV0Lm5hbWUiOiJrdWJlcm5ldGVzLWRhc2hib2FyZC10b2tlbi1uY2ZjcyIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VydmljZS1hY2NvdW50Lm5hbWUiOiJrdWJlcm5ldGVzLWRhc2hib2FyZCIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VydmljZS1hY2NvdW50LnVpZCI6IjkxODc4MDM5LWQwMDEtNGU0OC04NTU5LTgyZjUyMzI0NWYzNiIsInN1YiI6InN5c3RlbTpzZXJ2aWNlYWNjb3VudDprdWJlcm5ldGVzLWRhc2hib2FyZDprdWJlcm5ldGVzLWRhc2hib2FyZCJ9.UHqY8U8bhyAm5ms_7dP7S0zAX1BTg4k-rtG2leAsxG3yE2MtrvbVZumtTB67iZpcqjwIZPLVSnEae98ZlYu47dwbqdWWCtxaHq-4xOHHXVZc_9EBm5wJaPMbkdGCb2i6qGM0hAeHGb82b7ou2duaaApcpOixcJRGxL3ydjIF0HTYiSERz5xNiWcfK2nbLUf2g0XHcT7B5rICXs5ODFiKxtS2_6QTIY0SUz0T7_QOsLifc_rZfnZdEExb5iElJktFvxinpUtizp32y_BlsG2BFWExPZhn-arS6i07k8dmiepih4c9PbHmDLnNGn0r58Ogq6RoIvL7TiZar3p4VdKBOA

commande pour avoir le token:

           kubectl -n kubernetes-dashboard describe secrets kubernetes-dashboard-token-<TAB>
---------------------------------------------------------------
Partie2- EKS

micro-services EKS 
           http://ad4644d5587b5403599c612f2c35ff97-1951645112.us-east-2.elb.amazonaws.com/

------------------------------------------------------------------------------
Partie3- promethieux-grafana
        http://af206e311d0eb4ad6b0a6c19f970e965-1697783802.us-east-2.elb.amazonaws.com/ 
login: 
        admin 
password: 
        EKS!sAWSome 
lien direct
        http://af206e311d0eb4ad6b0a6c19f970e965-1697783802.us-east-2.elb.amazonaws.com/dashboards

--------------------------------------------------------------------------------------------
Partie4: argocd
            abbdcbed04bf14d119afa263636c0af2-319878540.us-east-2.elb.amazonaws.com

login 
     admin
pass:
           HIDehjWcWlGnsyUo
---------------------------------------------------------------------------------------------
Partie5: kube-bench

lancer les logs directement dans le node: 
        kube-bench --benchmark eks-1.0.1
à travers un job-kubectl 
        logs kube-bench-<value>(nom du pod)

--------------------------------------------------------------------------
mon git:
      https://github.com/IlhemBouazizi/ilhem/tree/main/micro-services
-------------------------------------------------------------------
mon compte aws:
            https://716949532148.signin.aws.amazon.com/console
User name: 
            lah
Pass: 
            80Kerwan
---------------------------------------------------------------------
