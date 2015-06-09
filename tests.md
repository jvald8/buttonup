1. GET / (200)
2. GET /account (401)
3. POST /login profile exists (201)   test admin user
4. GET /account (200)
5. POST /groups at least 1 object in response (201)
6. POST /login      new test user (201)
7. GET /account at least 1 object in pending group invites (200)
8. POST /account accept invitation (200)
9. GET /groups array of object IDs that user belogs to, one of which is the group object id which was just accepted an invitation to (200)
10.DELETE /account length of an array of group objects for a user === 0.
