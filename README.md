# Flask Prometheus Monitoring Sample

This project is a sample Flask application with Prometheus monitoring integration.

## Prerequisites

- Python 3.12 or higher
- pip (Python package installer)
- Postman (optional, for testing API endpoints)

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/flask-prometheus-monitoring-sample.git
   cd flask-prometheus-monitoring-sample
   ```

2. Create a virtual environment:
   ```
   python3 -m venv venv
   ```

3. Activate the virtual environment:
   - On macOS and Linux:
     ```
     source venv/bin/activate
     ```
   - On Windows:
     ```
     venv\Scripts\activate
     ```

4. Upgrade pip:
   ```
   pip install --upgrade pip
   ```

5. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Running the Application

To run the application, use the following command:

```
python app.py
```

The application will start and be available at `http://localhost:5000`.

## API Endpoints

The following endpoints are available:

- `GET /`: Root endpoint
- `POST /items`: Create a new item
- `GET /items/{item_id}`: Retrieve an item
- `PUT /items/{item_id}`: Update an item
- `DELETE /items/{item_id}`: Delete an item
- `GET /metrics`: Prometheus metrics endpoint

## Testing with Postman

A Postman collection is provided for testing the API endpoints. To use it:

1. Open Postman
2. Click on "Import" and select the `flask-metrics-postman-collection.json` file
3. The collection "Flask Metrics App" will be added to your Postman workspace
4. You can now use the requests to test each endpoint

## Monitoring

The application exposes Prometheus metrics at the `/metrics` endpoint. You can configure your Prometheus server to scrape these metrics for monitoring.

## Development

If you want to make changes to the project:

1. Ensure you're in the virtual environment (step 3 in Setup).
2. Make your changes to the `app.py` file or other relevant files.
3. Run the application to test your changes.

## Troubleshooting

If you encounter any issues:

1. Ensure you're using Python 3.12 or higher:
   ```
   python --version
   ```

2. Make sure all dependencies are correctly installed:
   ```
   pip install -r requirements.txt
   ```

3. Check that you're in the correct directory and the virtual environment is activated.

## Cleanup

When you're done working on the project:

1. Deactivate the virtual environment:
   ```
   deactivate
   ```

2. Optionally, remove the virtual environment directory:
   ```
   rm -rf venv
   ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.