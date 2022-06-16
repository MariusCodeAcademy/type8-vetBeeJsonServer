# json web server

[Paiskaitom](https://github.com/typicode/json-server#table-of-contents)

### jei reikia pasikeiskit porta package.json

## pets (sakykim petId === 98)

1. all pets
   `GET http://localhost:3000/pets`
2. single pet `GET http://localhost:3000/pets/98`
3. create a pet
   `POST http://localhost:3000/pets`
   ```
   {
   "name": "Mouse",
   "dob": "2017-01-01",
   "client_email": "test@example.com",
   "archived": false,
   }
   ```
4. delete a pet `PATCH http://localhost:3000/pets/98`

```
  {
  "archived": true,
  }
```

4. rename a pet `PATCH http://localhost:3000/pets/98`

```
  {
  "name": 'Mike',
  }
```

## logs

1. all logs
   `GET http://localhost:3000/logs`
2. single pet logs `GET http://localhost:3000/logs?pet_id=98`
3. create a log
   `POST http://localhost:3000/logs`
   ```
   {
    "pet_id": 98,
    "description": "broken leg",
    "status": "healed"
   }
   ```

## prescriptions

1. all prescriptions
   `GET http://localhost:3000/prescriptions`
2. single pet prescriptions `GET http://localhost:3000/prescriptions?pet_id=98`
3. create a prescription
   `POST http://localhost:3000/prescriptions`
   ```
   {
    "pet_id": 98,
    "comment": "for the best",
    "medication_id": 1
   }
   ```

## meds

taip pat kaip pets viskas.
