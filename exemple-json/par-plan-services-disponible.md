# (Par Plan) services disponible

## Services disponible

<mark style="color:green;">`GET`</mark> `/services_plan.php/?apikey=API_KEY`

**Headers**

| Name         | Value                         |
| ------------ | ----------------------------- |
| Content-Type | `application/json`            |
| apikey       | `votre api`                   |
| planname     | free/basique/standard/premium |

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "success": true,
  "plan": "Free",
  "services": [
    "collection_spotify",
    "collection_hotmail",
    "collection_mega",
    "collection_putalocura",
    "collection_crunchyroll",
    "collection_max",
    "collection_hbo",
    "collection_geoguessr",
    "collection_tunnelbear"
  ]
}
```
{% endtab %}

{% tab title="API non valide" %}
```
{
  "error": "Votre apikey est pas valide"
}
```
{% endtab %}

{% tab title="API non fournit" %}
```
{
  "error": "Merci de fournir une apikey"
}
```
{% endtab %}

{% tab title="Service Not Valid" %}
```
{
  "error": "No services found for the specified plan"
}
```
{% endtab %}
{% endtabs %}

```
Pour les erreurs, vérifier la documentation de la requête verify
```
