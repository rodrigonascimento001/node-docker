# node-docker
 
### 1. Limpar tudo que não está em uso (containers, networks, imagens dangling e cache):
```bash
docker system prune
```

### 2. Para remover tudo, incluindo imagens não utilizadas (não apenas dangling):
```bash
docker system prune -a
```

### 3. Para não ser perguntado para confirmar:
```bash
docker system prune -a -f
```

### 4. Remover apenas containers parados:
```bash
docker container prune
```

### 5. Remover apenas imagens dangling (sem tag):
```bash
docker image prune
```

### 6. Remover todas as imagens não utilizadas:
```bash
docker image prune -a
```

### 7. Remover volumes não utilizados:
```bash
docker volume prune
```

### 8. Remover networks não utilizadas:
```bash
docker network prune
```

---

**Dica:**  
Use o comando abaixo para liberar o máximo de espaço possível:
```bash
docker system prune -a --volumes
```
Isso remove tudo que não está em uso, incluindo volumes.

 