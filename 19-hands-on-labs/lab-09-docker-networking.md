# Lab 09: Docker networking

## Difficulty
Intermediate

## Estimated completion time
30 minutes

## Learning objectives
- Understand bridge networks
- Inspect container interfaces
- Observe how containers connect to each other

## Commands
```bash
docker network ls
docker run --rm --network bridge alpine ip addr
```

## Questions
1. What network mode did the container use?
2. What IP address did it receive?
3. Why does container networking differ from host networking?
