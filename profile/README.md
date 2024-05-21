# Greeve
<img src="https://github.com/Alterra-Greeve/.github/assets/133726246/3a58ead2-7977-4f31-8f29-bb54e55dc34b" width="350" />



![Static Badge](https://img.shields.io/badge/go-documentation-blue)
![Static Badge](https://img.shields.io/badge/refrences-blue?logo=go&labelColor=black)


Greeve is an innovative app that aims to increase user awareness and participation in environmental conservation and make it easier to purchase eco-friendly environmental goods and tools. The app not only offers a platform to purchase environmental goods and tools, but also provides information on the impact of users' activities on the environment as well as how to measure and reduce that impact.

## Feature Overview
- User Can Add Item to Shooping Cart
- User Can Cancel and Update Item From Shooping Cart
- User Can View Transaction Detail
- User Can Start Forum Discusion
- User Can View and Participate To Join Challange
- User Can Claim rewards and Voucher
- Admin Can Create Update Delete Product
- Admin Can Create Challenge
- Admin Create Impact Categories
- Admin Make Voucher

## API Reference

#### User

#### Get all Product
```http
  GET /api/products 
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### User Add to Shooping Cart
```http
  post /api/carts 
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `product_id` | `string` | **Required**. Id Product |

#### User Update Item on Shooping Cart
```http
  put /api/carts 
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `product_id` | `integer` | Id Product |

#### Admin
#### Post Product
```http
  POST /api/products
```

| Parameter   | Tipe     | Deskripsi                         |
| :---------- | :------- | :-------------------------------- |
| `name`      | `string` | **Required**. Nama produk baru.     |
| `price`     | `integer` | **Required**. Harga produk baru.    |
| `description` | `string` | Deskripsi produk baru.           |
| `image_url` | `string` | URL gambar produk baru.          |

## Guide

### Instalation
```bash
  go get -u github.com/greeve/v1
```
