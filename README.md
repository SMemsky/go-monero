# MONERO-API

## Note
This project is in slow development for my personal projects. Examples might or might not work.
You can always open an issue in case of something or try contacting me in Telegram: @Dexter3000

### For exmple daemon:

```
daemon := monero.NewDaemonClient("http://127.0.0.1:18081/json_rpc")
blockCount, err := daemon.GetBlockCount()
if err != nil {
    fmt.Println(err)
     return
} 
fmt.Println("Count:", blockCount)

```

### For exmple wallet:
```
wallet := monero.NewWalletClient("http://127.0.0.1:18082/json_rpc", "user", "pass")
balance, err := wallet.GetBalance()
if err != nil {
	fmt.Println(err)
	return
}
fmt.Println("balance:", balance)
```
