# Theia Helm Chart

Este repositório contém um Helm Chart para implantar [Theia] - uma plataforma extensível para desenvolvimento integrado.

## Estrutura do Chart

```
theia-chart/
|-- theia/
|-- templates/
|   |-- deployment.yaml
|   |-- _helpers.tpl
|   |-- configmap.yaml
|   |-- hpa.yaml
|   |-- ingress.yaml
|   |-- pvc.yaml
|   |-- secret.yaml
|   |-- service.yaml
|   |-- serviceaccount.yaml
|-- values.yaml
|-- questions.yaml
|-- Chart.yaml
|-- README.md
```

- **theia/:** Contém os recursos específicos da aplicação Theia.
- **templates/:** Contém os modelos do Kubernetes YAML para os recursos.
  - **deployment.yaml:** Define a configuração do Deployment do Theia.
  - **_helpers.tpl:** Arquivo auxiliar contendo funções do Helm.
  - **configmap.yaml:** Configuração para o ConfigMap usado pelo Theia.
  - **hpa.yaml:** Configuração para o Horizontal Pod Autoscaler (HPA).
  - **ingress.yaml:** Configuração para o Ingress.
  - **pvc.yaml:** Configuração para o Persistent Volume Claim (PVC).
  - **secret.yaml:** Configuração para o Secret.
  - **service.yaml:** Configuração para o Service.
  - **serviceaccount.yaml:** Configuração para a Service Account.
- **values.yaml:** Arquivo que define os valores padrão utilizados no Chart.
- **questions.yaml:** Perguntas frequentes e respostas relacionadas ao Chart.
- **Chart.yaml:** Metadados do Chart, incluindo versão e descrição.

## Como Usar

1. Clone este repositório:

```bash
git clone https://github.com/Contagiovaneines/theia.git
cd theia
```

2. Personalize os valores no arquivo `values.yaml` conforme necessário.


## Configurações Personalizadas

Consulte o arquivo `values.yaml` para ver as configurações disponíveis e suas descrições.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas (issues) ou enviar pull requests.

## FAQ

Consulte o arquivo `questions.yaml` para obter respostas às perguntas frequentes relacionadas a este Chart.
