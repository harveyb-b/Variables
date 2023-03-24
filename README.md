# Variables

            string url = $"https://api.openweathermap.org/data/2.5/forecast?q={location}&units=metric&appid=a4c5fa0aea885e9ddd149fb3e7bc3b40";
            
            string json = new WebClient().DownloadString(url);
            
            dynamic data = JsonConvert.DeserializeObject(json);
