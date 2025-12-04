# Redis Commands

## Strings (cache)
SET session:user1 "logged"
EXPIRE session:user1 300

## Hashes (carritos)
HSET cart:1 item1 2 item2 1
HGETALL cart:1

## Lists (cola de pedidos)
LPUSH pedidos "orden_1"
LPUSH pedidos "orden_2"
LRANGE pedidos 0 -1

## Sets (categorías)
SADD categorias "tech" "home"
SMEMBERS categorias

## Sorted Sets (ranking productos)
ZADD ranking 500 "Laptop"
ZADD ranking 200 "Mouse"
ZRANGE ranking 0 -1 WITHSCORES
