<!-- README.md -->

<h1 align="center">moverq1337</h1>

<p align="center">
  <b>Backend Go</b> • <b>DevOps</b> • строю сервисы, которые деплоятся без боли и живут в проде нормально 😎
</p>

<p align="center">
  <a href="https://t.me/moverq1337"><img src="https://img.shields.io/badge/Telegram-subscribe-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" /></a>
</p>

<p align="center">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=900&center=true&vCenter=true&width=1600&lines=Backend+%E2%86%92+Go%2FGin%2FGORM%2FgRPC%2FProtobuf%2FJWT;Data+%E2%86%92+PostgreSQL%2FSQL%2FMigrations%2FRedis%2FKafka%2FMinIO%2FClickHouse;Infra+%E2%86%92+Linux%2FNginx%2FTraefik%2FPangolin%2FCertbot;DevOps+%E2%86%92+Docker%2FCompose%2FGitLab+CI%2FJenkins%2FTerraform%2FAnsible%2FHelm;Observability+%E2%86%92+Prometheus%2FGrafana" />
</p>

---

## 👤 About
I’m **Tseretyan Georgiy**. I build **Go backends and DevOps infrastructure**: APIs, databases, messaging/queues, CI/CD, Kubernetes, and observability.<br>
**I like it when alerts are quiet, logs are useful, and deployments are boring.**

---

## 🧩 Stack
<p align="center">
  <img src="https://skillicons.dev/icons?i=go,apple,postgres,redis,docker,kubernetes,helm,terraform,githubactions,prometheus,grafana,nginx,linux&perline=7" />
</p>

---
```go
package main

import "fmt"

type Me struct {
	Handle string
	Backend, Data, Infra, DevOps, Obs []string
	Motto  string
}

func must(tag string, items ...string) string {
	return fmt.Sprintf("%-12s %v", tag+":", items)
}

func main() {
	me := Me{
		Handle: "moverq1337",
		Backend: []string{"Go", "Gin", "GORM", "gRPC", "Protobuf", "JWT"},
		Data:    []string{"PostgreSQL", "SQL", "Migrations", "Redis", "Kafka", "MinIO", "ClickHouse"},
		Infra:   []string{"Linux", "Nginx", "Traefik", "Pangolin", "Certbot"},
		DevOps:  []string{"Docker", "Compose", "GitLab CI", "Jenkins", "Terraform", "Ansible", "Helm"},
		Obs:     []string{"Prometheus", "Grafana"},
		Motto:   "quiet alerts • useful logs • boring deploys",
	}

	fmt.Println(">>> whoami:", me.Handle)
	fmt.Println(must("backend", me.Backend...))
	fmt.Println(must("data", me.Data...))
	fmt.Println(must("infra", me.Infra...))
	fmt.Println(must("devops", me.DevOps...))
	fmt.Println(must("obs", me.Obs...))
	fmt.Println(">>> motto:", me.Motto)
}

