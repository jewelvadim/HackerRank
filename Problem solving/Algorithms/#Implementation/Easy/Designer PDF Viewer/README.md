# [Designer PDF Viewer](https://www.hackerrank.com/challenges/designer-pdf-viewer)

**Solution**
<br>
```python
def designerPdfViewer(h, word):
    return max((h['abcdefghijklmnopqrstuvwxyz'.index(i)] for i in set(word))) * len(word)
```

If it is useful for you - I am happy. Please, press **star**.
<br>
If you know, how to make my solution better - please, text me.
