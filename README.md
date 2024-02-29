# Automate Kubernetes Deployment

![Screenshot 2024-02-29 at 10 47 14](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/35fb3a8c-f105-492b-b4f9-85da0a200e66)

we do terraform init and terraform apply:

![Screenshot 2024-02-29 at 14 30 08](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/cf0d1ca5-4caa-465e-89fc-268e3baa1b43)


we create a namespace in EKS Cluster:

![Screenshot 2024-02-29 at 14 43 27](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/ab19af2a-8ec3-41ff-ac5e-cfeafc14caa7)


we install the requirements:

![Screenshot 2024-02-29 at 14 42 00](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/accf2d60-edc5-43e8-847a-52effa08b994)


![Screenshot 2024-02-29 at 14 41 48](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/75a214a0-f638-4f58-9e49-9266eabc487e)

we execute the playbook:

![Screenshot 2024-02-29 at 14 42 42](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/79aa8854-45fb-416b-92cd-65125ff7eb41)


![Screenshot 2024-02-29 at 14 42 52](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/1ce01777-e474-4a8d-93ff-0324058b1c53)

we check that the namespace was created:

![Screenshot 2024-02-29 at 14 45 13](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/2c672952-49ce-4870-a439-c5f2c327fe01)

We will deploy that app in the new namespace:

![Screenshot 2024-02-29 at 14 48 10](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/ad4c35bb-1fd9-4136-8c3d-e07133b624a1)

we check the pod is running:

![Screenshot 2024-02-29 at 14 48 28](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/875979ed-4fb2-4eb3-a794-d5ac901055f9)


![Screenshot 2024-02-29 at 14 49 21](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/a97db1a2-7e3b-4b8f-acf9-88fd8a7fec55)

and finally we set the environment variable for kubeconfig:

![Screenshot 2024-02-29 at 14 51 33](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/65e2f1b2-6f16-423e-a3e7-df59da2a1346)

![Screenshot 2024-02-29 at 14 52 12](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/497aba0d-322a-404b-94b6-ed7b1ac53dbd)

and we remove kubeconfig from the tasks:

![Screenshot 2024-02-29 at 14 52 50](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/229d463a-1828-425c-89eb-d3145fc6e3b2)

![Screenshot 2024-02-29 at 14 53 43](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/db81f12c-d92c-4ac5-9734-cf832907a785)

if now we execute the ansible playbook it should be able to connect to the cluster:

![Screenshot 2024-02-29 at 14 53 59](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/33328e82-dc38-46a7-a79c-0cda47fad296)

![Screenshot 2024-02-29 at 14 52 32](https://github.com/redjules/Automate-Kubernetes-Deployment/assets/106017493/198bfa89-9ed5-4467-b919-a537edacc2f6)


and it does!
