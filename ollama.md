# OLLAMA

## Stop immediately
```bash
systemctl stop ollama
```

## Disable autostart on boot (stays off after reboot)
```bash
systemctl disable ollama
```

## Start manually when needed
```bash
systemctl start ollama
```

## Re-enable autostart on boot
```bash
systemctl enable ollama
```

## Check status
```bash
systemctl status ollama
```
```bash
systemctl is-enabled ollama
```
```bash
systemctl is-active ollama
```

## Update Ollama
```bash
curl https://ollama.ai/install.sh | sh
```

## List all Ollama models
```bash
ollama list
```

## Download & run models
```bash
ollama pull model
ollama run model
```

## Delete models
#### Delete model (frees up disk space)
```bash
ollama rm model
```
#### Unload model from RAM (does not delete it)
```bash
ollama stop model
```
