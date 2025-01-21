### Hi there 👋

![](https://github-readme-stats.vercel.app/api/top-langs/?username=sherlockzzw&show_icons=true&layout=compact&theme=vue&hide_border=true&hide=html,css)

### It always seems impossible until it's done.

![PHP](https://img.shields.io/badge/-PHP-00ADD8?style=flat-square&logo=php&logoColor=white)
![Golang](https://img.shields.io/badge/-Golang-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/-Python-00ADD8?style=flat-square&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-00ADD8?style=flat-square&logo=docker&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-00ADD8?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-00ADD8?style=flat-square&logo=redis&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/-Elasticsearch-00ADD8?style=flat-square&logo=elasticsearch&logoColor=white)
![Kafka](https://img.shields.io/badge/-Kafka-00ADD8?style=flat-square&logo=apache-kafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/-RabbitMQ-00ADD8?style=flat-square&logo=rabbitmq&logoColor=white)

---

### About Me

```go
package main

import (
	"fmt"
	"time"
)

func main() {
	selfIntroduction()
	for _, v := range selfIntroduction() {
		println(v)
	}
}

func selfIntroduction() map[string]string {
	sherlock := make(map[string]string)
	sherlock["name"] = "Sherlock"
	sherlock["age"] = getAge()
	sherlock["Learning"] = "PHP, GOLANG, JAVA, PYTHON"

	return sherlock
}

func getAge() string {
	start := time.Date(1998, 2, 28, 0, 0, 0, 0, time.Local)
	now := time.Now()

	years := now.Year() - start.Year()
	if now.YearDay() < start.YearDay() {
		years--
	}

	return fmt.Sprintf("%d", years)
}
