# Лабораторная работа 2 (Azure) - 3 вариант

Мартынюк Алексей (ППА1)

## Цель

Знакомство с наиболее популярными облачными сервисами и их Российскими аналогами, изучение возможностей для миграции на отчественные платформы. Понимание уровней абстрации над инфраструктурой в облаке.

## Предупреждение

Многие (читать: большинство) из представленых описаний и иллюстраций взяты (и переведены) с официальных страниц соответствующих сервисов.

## Сервисы Azure

**Machine Learning** – облачный сервис для развертывания моделей машинного обучения, основными преимуществами являются: легкое создание и тестирование, обучение на больших объемах данных и возможность масштабирования.

**SQL Data Warehouse** – управляемое хранилище данных. 

**Functions** - это сервис для создания и администрирования веб-приложений. Предоставляет множество удобных возможностей масштабирования, в том числе автоматизацию развертывания на принципах CI/CD. 

**Insight and Analytics** - это сервис, позволяющий управлять производительностью приложений, посредством сбора данных о работе серверов. 

**Key Vault** - это сервис для хранения ключей, сертификатов, секретов. С помощью него можно шифровать ключи и секреты.

**Logic Apps** - это сервис, который позволяет автоматизировать рабочие процессы. Предусмотрен визуальный конструктор, для автоматизации почти не требуется кода.

**ML API Service** - это сервис, который позволяет решать различные задачи в различных областях с помощью искусственного интеллекта. Из очевидных плюсов, простой способ интеграции ИИ в приложения и сервисы. 

**Network** - это сервис, который позволяет управлять сетевой инфраструктурой в облаке, а также создавать её. 

**Recovery services** - это сервис для хранения различных данных, чаще всего это бэкапы сервисов, конфигурации сервисов.

**Signal service** - это сервис, упрощающий добавление веб-функций в реальном времени. Например, необходимо отправить обновление подключенным клиентам, с помощью этого сервиса клиенты будут обновляться без необходимости опрашивания сервера. В целом, сервис может использоваться в любом сценарии, где требуется передавать данные с сервера клиенту в реальном времени. 

**Storage** - хранилище для различных видов данных.

**Media** - это сервис, для предоставления клиентам доступа к контенту на любых устройствах. Также содержимое защищается технологией DRM. 

**Devices** - это сервис для управления и отслеживания устройств в интернете вещей.

**Batch** - используется для эффективного выполнения пакетных заданий для параллельных и высокопроизводительных вычислений.

**Cognitive sevices** - сервис облачных API для внедрения предварительно обученных моделейв в проекты.

## Российские аналоги и их описание

**Yandex DataSphere** - отечественный облачный сервис для ML разработки.

**Yandex Managed Service for MySQL** - отечественный облачный сервис для развертывания и поддержки кластеров серверов MySQL.

**Cloud.ru FunctionGraph** - отечественный облачный сервис, позволяющий размещать и запускать код в бессерверной среде. Простыми словами, это значит, что не нужно будет покупать или арендовать оборудование.

**Yandex Monitoring** - отечественный облачный сервис, который позволяет собирать и отслеживать различные метрики облачных ресурсов.

**Yandex Lockbox** - отечественный облачный сервис для хранения ключей, сертификатов, секретов. 

**Cloud.ru Orchestration Service** - отечественный облачный сервис, который автоматизирует подготовку облачных ресурсов и развертывание приложений.

**YandexGPT API** - отечественный сервис, позволяющий решать задачи с помощью искусственного интеллекта.

**Yandex Virtual Private Cloud** - отечественный сервис для создания облачных сетей.

**Cloud.ru Server Migration Service** - отечественный сервис, позволяющий мигрировать P2V и V2V, помогающий в переносе локальных физических серверов.

**Yandex Object Storage** - отечественный универсальный сервис для облачного хранения.

**Yandex IoT Core** - отечественный сервис интернета вещей для обмена сообщениями по протоколу MQTT.

**Yandex Compute Cloud** - отечественный сервис, предоставляющий вычислительные мощности, который можно масштабировать.

**YandexGPT** - большая языковая модель от Yandex, которая позволяет генерировать текст в ответ на введенный запрос.

## Таблица и сопоставление с российскими аналогами

Для удобного сопоставления с российскими сервисами был заполнен столбец **Service Usage Type**.

**Machine Learning** - Yandex DataSphere

**SQL Data Warehouse** - Yandex Managed Service for MySQL

**Functions** - Cloud.ru FunctionGraph

**Insight and Analytics** - Yandex Monitoring

**Key Vault** - Yandex Lockbox

**Logic Apps** - Cloud.ru Orchestration Service

**ML API Service** - YandexGPT API

**Network** - Yandex Virtual Private Cloud

**Recovery services** - Cloud.ru Server Migration Service

**Signal service** - есть только иностранные аналоги

**Storage** - Yandex Object Storage

**Media** - есть только иностранные аналоги

**Devices** - Yandex IoT Core

**Batch** - Yandex Compute Cloud

**Cognitive sevices** - в случае с использованием, которое написано в таблице, (QnA) подходит YandexGPT, но полного аналога нет

| Service Usage Type                                    | Meter Category               | Meter Sub-Category       | Meter Name                  | Consumed Service                         | Russian Analogue                  |
|-------------------------------------------------------|------------------------------|--------------------------|-----------------------------|------------------------------------------|-----------------------------------|
|                                                       | Data Services                |                          |                             |                                          |                                   |
| Standartd tier of Sql services                        | SQL Data Warehouse           | Compute Optimized%       | 100 DWUs                    | Microsoft.Sql                            | Yandex Managed Service for MySQL  |
| Web apps execution on cloud                           | Functions                    |                          | %Execution%                 | Microsoft.Web                            | Cloud.ru FunctionGraph            |
| Control of work duration                              | Functions                    |                          | %Duration                   | Microsoft.Web                            | Cloud.ru FunctionGraph            |
| Analitics of data included per node                   | Insight and Analytics        |                          | Data Included per Node      | microsoft.operationalinsights            | Yandex Monitoring                 |
| Analitics of data overage per node                    | Insight and Analytics        |                          | Data Overage per Node       | microsoft.operationalinsights            | Yandex Monitoring                 |
| Collect, search and visualize machine data            | Insight and Analytics        |                          | Node                        | microsoft.operationalinsights            | Yandex Monitoring                 |
| Key management                                        | Key Vault                    |                          |                             | Microsoft.KeyVault                       | Yandex Lockbox                    |
|                                                       | Integration                  |                          |                             |                                          |                                   |
| Low code systems deployment                           | Logic Apps                   |                          |                             | Microsoft.Logic                          | Cloud.ru Orchestration Service    |
| Standartd tier of Machine learning services           | Machine Learning Service     | Model Management         | %Tier                       | Microsoft.MachineLearningModelManagement | Yandex DataSphere                 |
| Standard Workspace fee                                | Machine Learning Studio      |                          | Standard Workspace fee      | Microsoft.MachineLearning                | Yandex DataSphere                 |
| Standard Experiment Compute                           | Machine Learning Studio      |                          | Standard Experiment Compute | Microsoft.MachineLearning                | Yandex DataSphere                 |
| AI text analytics                                     | ML API Services              | Text Analytics           | Free                        | Microsoft.CognitiveServices              | YandexGPT API                     |
| Standart emotion API usage                            | ML API Services              | ML API Services          | Standard Emotion API%       | Microsoft.CognitiveServices              | YandexGPT API                     |
| Free mobile services                                  | Mobile Services              | Mobile Services          | Free Mobile Services        |                                          |                                   |
| Provide VPN gateway                                   | VPN Gateway                  |                          | %Gateway%                   | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Provide VPN gateway                                   | VPN Gateway                  |                          | %Gw%                        | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Provide data transfer inside virtual personal network | VPN Gateway                  |                          | %Data Transfer%             | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Creating endpoints associated with domain names       | Traffic Manager              |                          | %Azure Endpoint%            | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Creating endpoints connected with services            | Traffic Manager              |                          | %Service Endpoint%          | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Fast DNS queries perfomance                           | Traffic Manager              |                          | %DNS Queries%               | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Evaluating real user measurements                     | Traffic Manager              |                          | %Real User Measurements     | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Getting traffic view from network services            | Traffic Manager              |                          | %Traffic View%              | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Simplifying security deployment                       | Azure Firewall               |                          | Deployment                  | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| Analitics of processed data                           | Azure Firewall               |                          | Data Processed              | Microsoft.Network                        | Yandex Virtual Private Cloud      |
| VM replicated to Azure                                | Azure Site Recovery          |                          | VM _eplicated to Azure      | Microsoft.RecoveryServices               | Cloud.ru Server Migration Service |
| Chatbot for QnA                                       | Cognitive Services           | QnA Maker                |                             | Microsoft.CognitiveServices              | YandexGPT                         |
|                                                       | SignalR                      |                          |                             | Microsoft.SignalRService                 |                                   |
| Operations                                            | Event Grid                   |                          | Operations                  |                                          |                                   |
| Gateway to transfer data out of Azure                 | Windows Azure - All Services | All                      | Data Transfer Out%          | Microsoft.Storage                        | Yandex Object Storage             |
|                                                       | Media Services               |                          |                             | microsoft.media                          |                                   |
|                                                       | IoT Hub                      |                          |                             | Microsoft.Devices                        | Yandex IoT Core                   |
| Compute job scheduling                                | Virtual Machines             |                          |                             | Microsoft.Batch                          | Yandex Compute Cloud              |
| A series basic level VM                               | Virtual Machines             | A Series Basic%          |                             | %Compute                                 | Yandex Compute Cloud              |
| Entry level VM                                        | Virtual Machines             | A%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| Economic burstable VMs                                | Virtual Machines             | B%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| General purpose compute                               | Virtual Machines             | D%                       | D1/%                        | %Compute                                 | Yandex Compute Cloud              |
| General purpose compute                               | Virtual Machines             | D%                       | D1 %                        | %Compute                                 | Yandex Compute Cloud              |
| General purpose compute                               | Virtual Machines             | D%                       | D1%                         | %Compute                                 | Yandex Compute Cloud              |
| General purpose compute                               | Virtual Machines             | D%                       | D%                          | %Compute                                 | Yandex Compute Cloud              |
| Optimized for in-memory compute                       | Virtual Machines             | E%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| Compute optimized VMs                                 | Virtual Machines             | F%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| Compute optimized VMs                                 | Virtual Machines             | Standard_F4 VM (Windows) | Compute Hours               | %Compute                                 | Yandex Compute Cloud              |
| Memory and storage optimized VMs                      | Virtual Machines             | G%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| High Performance Computing VMs                        | Virtual Machines             | H%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| Storage optimized VMs                                 | Virtual Machines             | L%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| Memory optimized VMs                                  | Virtual Machines             | M%                       |                             | %Compute                                 | Yandex Compute Cloud              |
| GPU enabled VMs                                       | Virtual Machines             | N%                       |                             | %Compute                                 | Yandex Compute Cloud              |
|                                                       | Virtual Machines             | S%                       |                             | %Compute                                 | Yandex Compute Cloud              |

## Вывод

В ходе работы я познакомился с некоторыми из наиболее популярных облачных сервисов Azure, а также существующими Российскими аналогами. Действительно, большинство зарубежных сервисов могут быть заменены отечественными сервисами. В то же время, некоторые продвинутые сервисы (например, Signal service или Media) могут быть единственными в своем роде. 
