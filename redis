resource "azurerm_redis_cache" "positive11" {
  name                = "redis${random_id.server.hex}"
  location            = azurerm_resource_group.example.location
  resource_group_name = azurerm_resource_group.example.name
  capacity            = 1
  family              = "P"
  sku_name            = "sk_test_51L53TeSBwzby5YcBooVe7xqrw9DrV7SWyW5WKKYGSFO4fNSoDyd167DZrmIW6lZE6pHUDrYe9zfqGnCHTQUKhnPc00eL5w5pxY"
  enable_non_ssl_port = false

  redis_configuration {
    maxclients         = 256
    maxmemory_reserved = 2
    maxmemory_delta    = 2
    maxmemory_policy   = "allkeys-lru"
  }
}
