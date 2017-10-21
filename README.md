# HW20171021

public class Test1 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}
 public  class TestAnother1 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}

public 是公開的的類別，一個.java檔只能有一個公開的類別，如果有兩個public，解決方法是:
1.消除或刪除另外一個public
2.開新的類別，建立另外一個public

        class TestAnother1 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

public class Testing2 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}

若檔案名稱為Test2.java，而公開類別檔案名稱Testing2的話會導致系統找不到檔案而錯誤，解決的方法是:
公開類別檔案名稱必須要和檔案名稱相同

public class Test2 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

public class Test3 {
  public static void main(String args) {
    System.out.println("What's wrong with this program?");
  }
}

[]定義類別的語法參數列，反之則系統無法顯示輸出，解決的方法是:
[]重新輸出的String args兩個中間而擇一

public class Test3 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}

public class Test3 {
  public static void main(String args[]) {
    System.out.println("What's wrong with this program?");
  }
}

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

public class Test4 {
  public void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}

static 而是將類別名稱轉為作為名稱空間，透過類別名稱與、運算子來存取，System.out主要關聯是類別名稱static，若沒有static的話System.out取出存取類別名成和運算子，解決的方法是:

重新輸入static讓System.out有地方存取類別名稱和運算子取出並顯示

public class Test4 {
  public static void main(String[] args) {
    System.out.println("What's wrong with this program?");
  }
}
