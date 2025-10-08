# Added Information
With the .zpi file, unzip it to then run where the only thing you would need includes docker and .NET on your system, the rest is done for you with the code

To run, use something like postman and run commands such as get or post with this kind of URL http://localhost:5000/api/artist where you can replace artist with the other APIs but keep the rest. For post on postman, have a raw body and for each type of API data type, input the JSON data in there but you can personalise the JSON data

## These are the commands you need to run
- docker compose down --volumes --rmi all
- docker compose up --build -d

## Artifact Sample JSON
{
  "id": "6836a16869644d972a87f764",
  "title": "Exhibit A",
  "artistId": "6836a16869644d972a87f765",
  "productNo": "A001",
  "framed": true,
  "size": "24x36",
  "medium": "Oil on Canvas",
  "price": 1200,
  "salePrice": 1000,
  "onSale": true,
  "typeId": "6836a16869644d972a87f766",
  "type": {
    "id": "60f7b2c4e3a3f93d2c1d3d7e",
    "title": "Sculpture",
    "description": "Three-dimensional artworks carved or molded from various materials."
  },
  "colour": "Blue",
  "shape": "Rectangle",
  "new": false,
  "staffPicks": true,
  "exhibitionId": "6836a16869644d972a87f767",
  "artist": {
    "id": "6836a16869644d972a87f763",
    "name": "Test Artist",
    "dob": 1980,
    "born": "Darwin, NT",
    "languageGroup": "Group",
    "community": "Community",
    "description": "Description"
  },
  "exhibition": {
    "id": "60f7b2c4e3a3f93d2c1d3d7e",
    "title": "Exhibit A",
    "startDate": "2025-05-29T05:17:49.735Z",
    "endDate": "2025-05-29T05:17:49.735Z",
    "description": "Test A",
    "current": false
  }
}

## Artifact Type Sample JSON
{
  "id": "60f7b2c4e3a3f93d2c1d3d7e",
  "title": "Sculpture",
  "description": "Three-dimensional artworks carved or molded from various materials."
}

## Artist Sample JSON
{
  "id": "6836a16869644d972a87f763",
  "name": "Test Artist",
  "dob": 1990,
  "born": "Darwin, NT",
  "languageGroup": "Group",
  "community": "Community",
  "description": "Description"
}

## Exhibition Sample JSON
{
  "id": "60f7b2c4e3a3f93d2c1d3d7e",
  "title": "Exhibit A",
  "startDate": "2025-05-29T05:17:49.735Z",
  "endDate": "2025-05-29T05:17:49.735Z",
  "description": "Test A",
  "current": false
}
