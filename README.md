# Web3-Motoko-playground

This is a calculator created in the Motoko Playground. You can explore and interact with the project using the link below.

👉[Web3 Project](https://m7sm4-2iaaa-aaaab-qabra-cai.raw.ic0.app/?tag=1019490845)

```python
// Hesap makinesi
// Değişkenler (let -> immutable, var -> mutable)
// Operatörler
// Async metodu
// IF condition

// canister -> akıllı sözleşme

actor hesap_makinesi {
  var hucre: Int = 0;
  //toplama fonksiyonu
  public func toplama(s : Int) : async Int {
    hucre += s;
    hucre
    //Debug.Debug.print(debug_show (hucre));
  };

  //çıkarma fonksiyonu
  public func cikarma(s : Int) : async Int {
    hucre -= s;
    hucre
  };

  //çarpma fonksiyonu
  public func carpma(s : Int) : async Int {
    hucre *= s;
    hucre
  };

  //bölme fonksiyonu
  public func bolme(s : Int) : async ?Int {
    if (s==0){
      null
    } else{
      hucre /= s;
      ?hucre
    }
  };

  // Temizle
  public func temizle(): async() {
    hucre:=0;
  }
};
```
