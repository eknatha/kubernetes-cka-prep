# Pod Template

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-pod
  labels:
    app: nginx
spec:
  containers:
  - name: nginx
    image: nginx
    ports:
    - containerPort: 80
```
