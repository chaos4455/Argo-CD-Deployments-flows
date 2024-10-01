# 🚀 Argo-CD-Deployments-flows 🌐

[![GitOps](https://img.shields.io/badge/GitOps-ArgoCD-blue?style=flat&logo=argo&logoColor=white)](https://argo-cd.readthedocs.io/en/stable/) 
[![Kubernetes](https://img.shields.io/badge/Kubernetes-YAML-blue?style=flat&logo=kubernetes)](https://kubernetes.io/) 
[![KEDA](https://img.shields.io/badge/KEDA-scaling-green?style=flat&logo=kubernetes)](https://keda.sh/)

📄 Este repositório contém exemplos práticos de **YAMLs funcionais** para deploy de ambientes no Kubernetes utilizando práticas de **GitOps** com **ArgoCD** e **KEDA**, testados em cenários reais. Os exemplos são usados para **showcases**, demonstrando **downscaling** e **upscaling** dinâmico com **KEDA**, implementados em **Apache** e **Nginx**.

## 🧑‍💻 Sobre o Projeto
Aqui estão YAMLs completos que permitem o deploy de aplicações em Kubernetes com GitOps usando o ArgoCD. O foco é mostrar **escalabilidade horizontal automática**, integração com **CI/CD pipelines** e a implementação real de **GitOps**.

---

## 🔑 Funcionalidades Principais
- **Escalabilidade Automática** com [KEDA](https://keda.sh/) ⬆⬇
- **Deploy GitOps** com [ArgoCD](https://argo-cd.readthedocs.io/en/stable/) 🌟
- Configuração de **Ingress** para serviços externos 🚪
- Exposição pública de serviços com **LoadBalancer** ⚖️
- Testes em **Apache** e **Nginx** com **KEDA** 🧪

---

## 🌟 Showcase
Esses arquivos YAML foram testados em **deploys reais** no Kubernetes, incluindo:
- **[apache-argo-lean.yaml](https://github.com/chaos4455/Argo-CD-Deployments-flows/blob/main/argodeploy/apache-argo-lean.yaml)**: deploy de um servidor Apache com escalabilidade mínima e máxima, utilizando KEDA para auto-scale.
- **[minio.yaml](https://github.com/chaos4455/Argo-CD-Deployments-flows/blob/main/minio/minio.yaml)**: deploy do MinIO sem KEDA, para ambientes com necessidade de armazenamento distribuído.
- **[nginx.yaml](https://github.com/chaos4455/Argo-CD-Deployments-flows/blob/main/nginx/nginx.yaml)**: deploy de Nginx com KEDA, utilizando escalabilidade automatizada baseada em métricas de CPU.

---

## 📊 Arquitetura Utilizada
O repositório cobre múltiplos cenários, como:
- Deploy em namespaces dedicados no Kubernetes.
- Exposição pública via **Ingress** e **LoadBalancer**.
- Uso de métricas para escalabilidade dinâmica via **KEDA**.

---

## 🛠 Tecnologias Envolvidas
- **Kubernetes**: Plataforma de orquestração de containers.
- **ArgoCD**: Ferramenta para automação e controle de versões em ambientes GitOps.
- **KEDA**: Solução para auto-escalabilidade de workloads baseadas em eventos.
- **Nginx** e **Apache**: Servidores web configurados para escalabilidade horizontal.

---

## 📝 Estrutura do Repositório
- `argodeploy/`: Contém YAMLs para deploys utilizando **ArgoCD**.
  - [apache-argo-lean.yaml](https://github.com/chaos4455/Argo-CD-Deployments-flows/blob/main/argodeploy/apache-argo-lean.yaml): Arquivo de deploy do Apache com KEDA.
- `minio/`: YAML para deploy de **MinIO**, sem KEDA.
  - [minio.yaml](https://github.com/chaos4455/Argo-CD-Deployments-flows/blob/main/minio/minio.yaml): Deploy funcional do MinIO com LoadBalancer.
- `nginx/`: Exemplo de deploy com **Nginx** e escalabilidade via KEDA.
  - [nginx.yaml](https://github.com/chaos4455/Argo-CD-Deployments-flows/blob/main/nginx/nginx.yaml): Deploy de Nginx com Ingress e auto-escalabilidade.

## 🎯 Exemplo da ação de upscaling e downscaling em tempo real 
![K8Studio_OFyxsvQOPn](https://github.com/user-attachments/assets/0658d214-950e-49ee-8988-37b6e4257c22)
![K8Studio_N3JdBkzOkz](https://github.com/user-attachments/assets/c8fd24c8-1806-4035-a6a6-8551b80fffdb)
![K8Studio_Icn22lOnK9](https://github.com/user-attachments/assets/50c2c329-d391-4cf5-8592-0cce5b381192)
![K8Studio_BrV0OWA4pA](https://github.com/user-attachments/assets/78cbfa0a-a251-4f5c-a833-5c8bf4eb5d53)
![K8Studio_a5rJY0O4Bn](https://github.com/user-attachments/assets/c26989ec-ef10-4e3e-8bd3-54eb6e4bacfc)


## 🎯 Exemplo de upscaling e downscaling do apache 

![K8Studio_9RKrqsVnLP](https://github.com/user-attachments/assets/11582bf0-e5f7-4e20-8bac-965173c51d4c)
![K8Studio_9pxzZpBXq4](https://github.com/user-attachments/assets/f8b12f52-c585-4c20-9dba-f51f86b4c5c2)
![K8Studio_h3cL91Zy13](https://github.com/user-attachments/assets/e64227f9-1f49-47fa-8e7c-14c7962658d8)
![K8Studio_jRnHIqOd3X](https://github.com/user-attachments/assets/4bb3ecf3-6737-412f-827b-7adb729eab82)
![K8Studio_hn9bRtesrS](https://github.com/user-attachments/assets/2eea0df2-cf9e-4ed1-9a57-f6f8f061144a)

## 🎯 Exemplo de upscaling e downscaling do visto dentro do argocd 

![chrome_uAgleGCnKq](https://github.com/user-attachments/assets/2dfea64d-8b7e-4d50-9493-3b4dedfdabaa)
![chrome_OOUhtZ3QHL](https://github.com/user-attachments/assets/8b545f1b-9fcf-49bd-a6e6-5df5d37c83b8)
![chrome_uW7jeHFq3r](https://github.com/user-attachments/assets/515a6f48-0540-4834-a8a3-af64bb88cadb)
![chrome_adp9QPLTin](https://github.com/user-attachments/assets/e4483549-6ea5-4eda-a12d-7ce8c63d07cd)
![chrome_Yd4nQdpRWP](https://github.com/user-attachments/assets/cc3e1dca-a8af-41d4-a24e-ba73875dd249)

---

## 🧰 Como Usar
1. **Clone o repositório**:
    ```bash
    git clone https://github.com/chaos4455/Argo-CD-Deployments-flows.git
    ```
2. **Aplique os arquivos YAML** no seu cluster Kubernetes:
    ```bash
    kubectl apply -f <path_to_yaml>
    ```
3. Use o **ArgoCD** para controlar e monitorar os deploys via **GitOps**.

---

## 📸 Prints & Demonstrações
🖼️ Em breve, vou adicionar prints para mostrar visualmente o processo de deploy e a escalabilidade em tempo real. Fique atento!

---

## 🌐 Links Úteis
- [Documentação do ArgoCD](https://argo-cd.readthedocs.io/en/stable/)
- [Documentação do KEDA](https://keda.sh/docs/latest/)
- [Kubernetes](https://kubernetes.io/docs/home/)

---

## 🎯 Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

---

## 🛡️ Licença
Distribuído sob a licença **MIT**. Veja [LICENSE](./LICENSE) para mais detalhes.

---

**By Elias Andrade** | chaos4455 | [GitHub](https://github.com/chaos4455)
