# eventhub2cosmosdb_function

Azure Functions Event Hubs Message to CosmosDB

This Azure Function listens to messages from an Azure Event Hub and writes them to an Azure CosmosDB. It is designed to handle high-throughput event processing and ensure reliable message delivery to the database.

**Note:** This function has been tested with Python 3.11 only, as the Azure Functions Core Tools are not supported on higher releases.

## Setup

1. **Create a virtual environment**:
    ```bash
    python -m venv .venv
    ```

2. **Activate the virtual environment**:
    ```bash
    source .venv/bin/activate
    ```

3. **Initialize the Azure Function**:
    ```bash
    func init --python
    ```

4. **Clone or copy necessary files**:
    - `function_app.py`
    - `local.settings.json`
    - `requirements.txt`

5. **Update `local.settings.json`** with your configuration.

6. **Start the function locally**:
    ```bash
    func start
    ```

## Deployment

If the function is running successfully locally, you can deploy to an existing Azure function app:

```bash
func azure functionapp publish iotmessagemover
