# TheCashier

a. TheCashier
b. Aplikasi bisa menambahkan item dan menjumlah harga keseluruhan item
c. 

        public string getTitle()
        {
            return title;
        }
        public int getQuantity()
        {
            return quantity;
        }
        public string getType()
        {
            return type;
        }
        public double getPrice()
        {
            return price;
        }
        public double getSubTotal()
        {
            subtotal = price * quantity;
            return subtotal;
        }

method Item.cs digunakan untuk menghandle fungsi inputan user seperti mendapatkan nama item, jumlah item, jenis item, harga item


	private List<Item> listItem;
        private double total = 0;
        public Calculator()
        {
            this.listItem = new List<Item>();
        }
        public void addItem(Item item)
        {
            this.listItem.Add(item);
            this.total += item.getSubTotal();
        }
        public double getTotal()
        {
            return total;
        }
        public List<Item> getListItem()
        {
            return listItem;
        }


method Calculator.cs yang mengandung konsep single responsibility berfungsi untuk menambahkan inputan user ke dalam list dan kemudian dijumlah atau ditotal harganya.
