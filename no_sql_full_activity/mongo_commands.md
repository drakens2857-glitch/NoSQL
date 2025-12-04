# MongoDB Commands

## Crear colecciones
db.createCollection("usuarios")
db.createCollection("productos")
db.createCollection("ordenes")

## Inserts
db.usuarios.insertOne({ nombre: "Ana", email: "ana@mail.com" })
db.productos.insertMany([
  { nombre: "Laptop", precio: 1200, stock: 10 },
  { nombre: "Mouse", precio: 20, stock: 100 }
])

## Queries
db.productos.find()
db.productos.find({ precio: { $gt: 50 } })

## Updates
db.productos.updateOne({ nombre: "Laptop" }, { $set: { stock: 9 } })

## Deletes
db.productos.deleteOne({ nombre: "Mouse" })
