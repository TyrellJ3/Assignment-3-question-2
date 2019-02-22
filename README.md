# Assignment-3-question-2
public class Book {
   private String Name;
   private Author author;
   private double price;
   private int qtyInStock;

    public Book(String Name, Author author, double price, int qtyInStock) {
        this.Name = Name;
        this.author = author;
        this.price = price;
        this.qtyInStock = qtyInStock;
    }

    public String getName() {
        return Name;
    }

    public Author getAuthor() {
        return author;
    }

    public double getPrice() {
        return price;
    }

    public int getQtyInStock() {
        return qtyInStock;
    }

    public void setPrice(double price) {
        this.price = price;
    }

    public void setQtyInStock(int qtyInStock) {
        this.qtyInStock = qtyInStock;
    }

    @Override
    public String toString() {
        return "Book{" + "Name=" + Name + ", author=" + author + ", price=" + price + ", qtyInStock=" + qtyInStock + '}';
    }
   
   public static void main(String[] args) {
  Author sipser = new Author ("Nicki Washington", "washingtonn@winthrop.edu", 'f');
  Book toc = new Book ("Theory of Computation", sipser, 200.00, 12);

// Book toc = new Book ("Theory of Computation", new Author
//("Michael Sipser", "msipser@mit.edu", 'm'), 200.00, 12);

   
       System.out.println(toc.getName());
       System.out.println(toc.getPrice());
       System.out.println(toc.getQtyInStock());


}
}
