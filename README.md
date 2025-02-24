# construction-smart-test
construction-smart-test

**Part 1 : Backend**

- Make sure all nuget package installed

- **appsettings.json**
"ConnectionStrings": {
    "DefaultConnection": "Host=localhost;Port=5432;Database=postgres;Username=postgres;Password=grafik123" // put your database connection string
  },
  "Kafka": {
    "BootstrapServers": "kafka-9644aa4-grafikyusvaaji-d9b0.k.aivencloud.com:19541",
    "Topic": "es.construction.hbx",
    "SaslMechanism": "PLAIN",
    "SecurityProtocol": "SASL_SSL", 
    "SaslUsername": "your_kafka_username",
    "SaslPassword": "your_kafka_password",
    "SslCaLocation": "your_project_path\\cert\\to\\ca-cert\\ca.pem"  // you can change with your own kafka settings
  },
  "ElasticSearch": {
    "Uri": "http://localhost:9200", // make sure elasticsearch services running on this Uri
    "DefaultIndex": "constructionprojects" // default index that used on elasticsearch services
  },
  "Jwt": {
    "Key": "your_new_secret_key_which_is_at_least_16_chars",
    "Issuer": "grafikIssuer",
    "Audience": "grafikAudience"
  }

**Part 2 : Front**
- Make sure all package installed (npm install / yarn )
- Make sure 
  baseURL: 'https://localhost:7051/api' is correct for comminication within **Backend**

  
