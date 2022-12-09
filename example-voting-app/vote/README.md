

## Image Build Info

| Item      | Description |   
| :---        |    :----:   |  
| Base  |  python:2.7-alpine  |  
| Work Directory  |  /app |    
| Build Instructions  |  pip install -r requirements.txt |
| Ports | 80 |  
| Launch Command | gunicorn app:app -b 0.0.0.0:80 |  
