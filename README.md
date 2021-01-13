# StudiKasus Nazil Alifurohman E.R. 19.11.2755

Program Aplikasi Promos ini adalah pengembangan dari aplikasi sebelumnya dengan menambahkan fitur baru

# Kegunaan
- User dapat melihat daftar makanan yang ditawarkan
- User dapat memasukkan atau menghapus makanan pilihan ke dalam keranjang
- User dapat melihat subtotal makanan yang terdapat pada keranjang
- User dapat melihat daftar voucher yang ditawarkan
- User dapat menggunakan salah satu voucher
- User dapat melihat harga total termasuk potongannya

# Alur Program
 User akan dihadapkan dengan tampilan dari MainWindow dengan isi subtotal, total harga, voucher, dan keranjang belanja. Disediakan pilihan berbagai item dan user bisa langsung
 mengklik maka item akan berada di keranjang belanja. Disediakan voucher bagi user yang bisa mengurangi total harga dari keranjang belanja. 
 Berikut adalah potongan code untuk menampilkan list item

        private void generateContentPenawaran()
        {
            Item coffeLate = new Item("Coffe Late", 30000);
            Item blackTea = new Item("BlackTea", 20000);
            Item pizza = new Item("Pizza", 75000);
            Item milkShake = new Item("Milk Shake", 15000);
            Item friedRice = new Item("Fried Rice Special", 45000);
            Item watermelonJuice = new Item("Watermelon Juice", 25000);
            Item lemonSquash = new Item("Lemon Squash", 30000);

            Penawarancontroller.addItem(coffeLate);
            Penawarancontroller.addItem(blackTea);
            Penawarancontroller.addItem(pizza);
            Penawarancontroller.addItem(milkShake);
            Penawarancontroller.addItem(friedRice);
            Penawarancontroller.addItem(watermelonJuice);
            Penawarancontroller.addItem(lemonSquash);

            listPenawaran.Items.Refresh();
        }
