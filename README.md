# Grinder

> Grinder (noun): a player that populates the lower lines or lower pairings. Has hands of stone, but is physical and works hard when he’s out on the ice. Usually beloved by the rest of the team.

Grinder is a Go based framework with the aim of making the development of microservices easier. It attempts to do all the hard work / heaving lifting, hence why we called it Grinder, so that you can focus on your service.

## Example
```go
func main() {
	svc := grinder.New()

	// index handler
	svc.GET("/", func(ctx grinder.Context) error {
		return c.String(200, "Legs feed the wolf")
	})

	svc.Start()
}
```