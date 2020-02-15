from appwrite.client import Client
from appwrite.services.teams import Teams

client = Client()

(client
  .set_project('5df5acd0d48c2')
)

teams = Teams(client)

result = teams.create_membership('[TEAM_ID]', 'email@example.com', {}, 'https://example.com')