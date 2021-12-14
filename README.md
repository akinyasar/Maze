# Maze
    Search Algorithms with Python
Python ile yazılmış bu uygulamada Arama Algoritmalarından Uninformed Search kategorisine giren Depth First Search (DFS) ve Breadth First Search (BFS) algoritmasını daha iyi anlayabilmek adına bir labirent problemi ele aldım. Oluşturulan 3 farklı labirentte bu iki algoritmanın nasıl çalıştığını inceleyebilirsiniz.
## Önemli Notlar
- Proje klonlandıktan sonra çalıştırmak için dosya dizinindeki terminale;

 ```python maze.py maze1.txt```

yazarak 1. labirent ile uygulamayı çalıştırabilirsiniz. maze1.txt yerine istenen labirent yazarak çalıştırılabilir. 
- Algoritmalar arası değişiklik yapmak için;
```python
def solve(self):
        """Finds a solution to maze, if one exists."""

        # Keep track of number of states explored
        self.num_explored = 0

        # Initialize frontier to just the starting position
        start = Node(state=self.start, parent=None, action=None)
        frontier = QueueFrontier()
        frontier.add(start)
```
fonksiyonundaki ```frontier = QueueFrontier()``` atamasını ```frontier = StackFrontier()``` olarak değiştirmelisiniz. Bu sayede algoritma BFS'den DFS'e geçmiş olacaktır.

- SearchAlgorithms.pptx dosyasında algoritmalar hakkında hazırladığım sunum bulunmaktadır.
