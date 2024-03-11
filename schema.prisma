model ProductCategory {
  id          Int      @id @default(autoincrement())
  name        VarChar(255) @unique
  desc        Text?
  createdAt   DateTime  @default(now())
  modifiedAt  DateTime  @updatedAt
}

model Product {
  id          Int      @id @default(autoincrement())
  name        VarChar(255)
  desc        Text?
  sku         VarChar(255)  @unique
  categoryId  Int      @db.ForeignKey("ProductCategory")
  inventory   Inventory?
  price       Decimal 
  discountId  Int?
  createdAt   DateTime  @default(now())
  modifiedAt  DateTime  @updatedAt
  deletedAt   DateTime?
  category    ProductCategory  @relation(fields: [categoryId], references: [id])
}

model Inventory {
  id          Int      @id @default(autoincrement())
  quantity    Int
  createdAt   DateTime  @default(now())
  modifiedAt  DateTime  @updatedAt
  deletedAt   DateTime?
}

