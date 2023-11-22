NAMA  : ALYA SEFHIA EKA PUTRI

KELAS: TI.22.B1

NIM  : 312210108

# TUGAS OOP PERTEMUAN 9 

1. Implementasikan dengan Bahasa Pemrograman diagram class berikut:

   ![Tugas 9](https://github.com/AkuuAlyaaa/OOP_PER_9/assets/115520278/30c9411b-e1f8-48dc-b9a2-ee064a65055f)

   - Source Code :

               using System;
          using System.Collections.Generic;
          using System.Linq;
          using System.Text;
          using System.Threading.Tasks;
          
          namespace Bangun_Datar
          {
              class BangunDatar
              {
                  public virtual float HitungLuas()
                  {
                      return 0;
                  }
          
                  public virtual float HitungKeliling()
                  {
                      return 0;
                  }
              }
          
              // Kelas turunan untuk persegi
              class Persegi : BangunDatar
              {
                  private int sisi;
          
                  public Persegi(int sisi)
                  {
                      this.sisi = sisi;
                  }
          
                  public override float HitungLuas()
                  {
                      return sisi * sisi;
                  }
          
                  public override float HitungKeliling()
                  {
                      return 4 * sisi;
                  }
              }
          
              // Kelas turunan untuk lingkaran
              class Lingkaran : BangunDatar
              {
                  private float jariJari;
          
                  public Lingkaran(float jariJari)
                  {
                      this.jariJari = jariJari;
                  }
          
                  public override float HitungLuas()
                  {
                      return (float)(Math.PI * jariJari * jariJari);
                  }
          
                  public override float HitungKeliling()
                  {
                      return (float)(2 * Math.PI * jariJari);
                  }
              }
          
              // kelas turunan untuk segitiga
          
              class Segitiga : BangunDatar
              {
                  private float alas;
                  private float tinggi;
                  private int sisi1;
                  private int sisi2;
                  private int sisi3;
          
                  public Segitiga(float alas, float tinggi, int sisi1, int sisi2, int sisi3)
                  {
                      this.alas = alas;
                      this.tinggi = tinggi;
                      this.sisi1 = sisi1;
                      this.sisi2 = sisi2;
                      this.sisi3 = sisi3;
                  }
          
                  public float Alas
                  {
                      get { return alas; }
                      set { alas = value; }
                  }
          
                  public float Tinggi
                  {
                      get { return tinggi; }
                      set { tinggi = value; }
                  }
          
                  public int Sisi1
                  {
                      get { return sisi1; }
                      set { sisi1 = value; }
                  }
          
                  public int Sisi2
                  {
                      get { return sisi2; }
                      set { sisi2 = value; }
                  }
          
                  public int Sisi3
                  {
                      get { return sisi3; }
                      set { sisi3 = value; }
                  }
          
                  public float HitungLuas()
                  {
                      return 0.5f * alas * tinggi;
                  }
          
                  public int HitungKeliling()
                  {
                      return sisi1 + sisi2 + sisi3;
                  }
              }
          
          
              class Program
              {
                  static void Main()
                  {
                      // Contoh penggunaan kelas Persegi
                      Persegi persegi = new Persegi(10);
                      Console.WriteLine("Persegi");
                      Console.WriteLine("Luas: " + persegi.HitungLuas());
                      Console.WriteLine("Keliling: " + persegi.HitungKeliling());
          
                      Console.WriteLine();
          
                      // Contoh penggunaan kelas Lingkaran
                      Lingkaran lingkaran = new Lingkaran(3.5f);
                      Console.WriteLine("Lingkaran");
                      Console.WriteLine("Luas: " + lingkaran.HitungLuas());
                      Console.WriteLine("Keliling: " + lingkaran.HitungKeliling());
          
                      Console.ReadLine();
          
                      // Contoh penggunaan kelas Segitiga
                      Segitiga segitiga = new Segitiga(5.5f, 8.5f, 4, 3, 6);
          
                      Console.WriteLine("Segitiga:");
                      Console.WriteLine("Luas: " + segitiga.HitungLuas());
                      Console.WriteLine("Keliling: " + segitiga.HitungKeliling());
          
                      Console.ReadLine();
          
                  }
              }
          }

   - Output :
  
     ![output](https://github.com/AkuuAlyaaa/OOP_PER_9/assets/115520278/77ba7235-bde5-499e-811d-238610d344e1)

Sekian...

Terimakasih...

     

