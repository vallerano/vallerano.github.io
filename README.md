team_name = "FC Vallerano"
location = "Rome"
foundation = 2020
colors = "black and green"

president = "Lorenzo Sulpizii"
vice_president = "Alessio Amatori"
ceo = "Samuele Zolarsi"
sporting_director = "Giancarlo De Marzo"
press_chief = "Simone Strani"
sponsors = ["Bar de Cenci", "Gype Sport", "Parrucchiere Zolarsi"]
players = ["Antonio Maria di Giulio", "Leonardo Cappellani", "Giuseppe Pirozzi", "Giulio Toletti"]

html = f"""
<html>
    <head>
        <title>{team_name}</title>
    </head>
    <body>
        <h1>{team_name}</h1>
        <p>Location: {location}</p>
        <p>Foundation: {foundation}</p>
        <p>Colors: {colors}</p>
        <h2>Hierarchy</h2>
        <p>President: {president}</p>
        <p>Vice President: {vice_president}</p>
        <p>CEO: {ceo}</p>
        <p>Sporting Director: {sporting_director}</p>
        <p>Press Chief: {press_chief}</p>
        <h2>Sponsors</h2>
        <ul>
"""

for sponsor in sponsors:
    html += f"<li>{sponsor}</li>"

html += """
        </ul>
        <h2>Key Players</h2>
        <ul>
"""

for player in players:
    html += f"<li>{player}</li>"

html += """
        </ul>
    </body>
</html>
"""

print(html)
