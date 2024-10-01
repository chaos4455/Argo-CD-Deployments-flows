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
