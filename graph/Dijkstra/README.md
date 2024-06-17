#  Giải thuật Dijkstra

- Ý tưởng:
  - có 2 cách để đến được node liền kề A -> B:
    - 1 đường đi trực tiếp A->B
    - 2 đường đi gián tiếp chắc node liền kề khác: A->C->..->B
    => Nếu A B gần nhau nhất => không có đường nào ngắn hơn để đi đến B


Giải thuật:
    1. bắt đầu từ node 0 -> update khoảng cách cho các node liền kề -> bỏ node 0 ra khỏi danh sách duyệt
    2. chọn node có khoảng cách bé nhất trong các node còn lại
    3. cập nhật khoảng cách cho các node liền kề của node được chọn -> bỏ node được chọn ra khỏi danh sách duyệt
       - Coi như gộp điểm được chọn vào gốc (stable) => các node liền kề của node được chọn coi như liền kề với gốc
    4. quay lại bước 2.



