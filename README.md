# eventhub2cosmosdb_function

Azure Functions Event Hubs Message to CosmosDB

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