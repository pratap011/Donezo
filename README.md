## User Journey for Adding an Item to the List

<img width="907" alt="image" src="https://github.com/user-attachments/assets/b5b4c189-a28f-4142-ade4-1c1d3a80fd20" />

## Sample ER Diagram 

<img width="907" alt="image" src="https://github.com/user-attachments/assets/66c2865c-8bb1-4e24-bd13-965f85c1b8c8" />

```mermaid
erDiagram
    User {
        string id "PK"
        string email
        string password "hashed"
        string full_name
        int created_on
        int updated_on
    }

    List {
        string id "PK"
        string type "TV_SHOWS,MOVIES,PODCASTS,GAMES,ANIME,CUSTOM"
        string name
        int completed_item_count
        int total_item_count
        string image_url
        string user_id "FK"
        int created_on
        int updated_on
    }

    Item {
        string id "PK"
        string external_id
        string name
        string status "PENDING,DONE"
        string image_url
        boolean is_finished
        int completed_episodes
        int total_episodes
        float completed_percentage
        string[] tags
        string list_id "FK"
        int created_on
        int updated_on
    }

    User ||--|{ List : has
    List ||--o{ Item : has
```