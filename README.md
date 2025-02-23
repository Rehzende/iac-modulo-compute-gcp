## Requerimentos

| Nome | Versão |
|------|---------|
| terraform | >= 1.0.0 |

## Providers

| Nome | Versão |
|------|---------|
| google | >=3.81.0 |

## Recursos

| Nome | Type |
|------|------|
| [google_compute_instance.default](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_instance) | resource |

## Entradas

| Nome | Descrição | Tipo | Padrão | Requerido |
|------|-------------|------|---------|:--------:|
| project | Nome do projeto existente na Google Cloud | `string` | n/a | sim |
| instance_name | Nome da instância na Google Cloud | `string` | n/a | sim |
| instance_image | Nome da instância na Google Cloud | `string` | n/a | sim |
| machine_type | Tipo de máquina na Google Cloud | `string` | n/a | sim |
| network | Nome da rede existente na GCP | `string` | n/a | sim |
| subnetwork | Nome da subrede existente na GCP * foi definido o valor padrão para caso passe a NETWORK com o valor 'default' | `string` | `""` | não |
| zone | Zona na Google Cloud | `string` | n/a | sim |
| labels | Mapa de labels para nossa instância maneira | `map(string)` | n/a | sim |
| tags | Lista de tags de rede associadas à instância | `list(string)` | n/a | sim |
| metadata_startup_script | Script executado na inicialização do Sistema Operacional | `string` | "" | não |

## Saídas

No outputs.
