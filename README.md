# Pet Store API Testing Project

This project contains a Postman collection for testing the Pet Store API. It includes various API endpoints for managing pets, orders, and inventory.

## Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (for Newman)
- [Postman](https://www.postman.com/downloads/)

## Installation

1. Clone this repository or download the `Pet-Store.postman_collection.json` file.

2. If you want to use Newman (command-line collection runner for Postman), install it globally using npm:

    ```npm install -g newman```

## Running the Tests

### Using Postman

1. Open Postman.
2. Click on "Import" in the top left corner.
3. Choose "File" and select the `Pet-Store.postman_collection.json` file.
4. Once imported, you'll see the "Pet-Store" collection in your Postman workspace.
5. Click on the "..." (ellipsis) next to the collection name and select "Run collection".
6. In the collection runner, you can choose which requests to run and set the environment if needed.
7. Click "Run Pet-Store" to execute the tests.

### Using Newman

1. Open a terminal or command prompt.
2. Navigate to the directory containing the `Pet-Store.postman_collection.json` file.
3. Run the following command:

    ```newman run Pet-Store.postman_collection.json```

4. Newman will execute all the requests in the collection and display the results in the terminal.

## Collection Structure

The collection includes the following requests:
- Add new pet
- Find pets by status
- Update existing pet
- Find pet by ID
- Return pet inventory
- Place an order for a pet
- Find order by ID
- Delete order by ID
- Delete pets

Each request includes pre-request scripts and tests to validate the responses.

## Variables

The collection uses the following variables:
- `baseURL`: Set to "https://petstore.swagger.io/v2"
- `petId`: Stores the ID of the created pet
- `orderId`: Stores the ID of the created order

Make sure these variables are set correctly before running the collection.

## Contributing

Feel free to fork this project and submit pull requests with any improvements or additional tests.

## License

This project is open source and available under the [MIT License](LICENSE).