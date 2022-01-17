package TULIPKU;

public class PetaniBunga extends Pesanan{
    private String nama_barang;

    public PetaniBunga(String alamat_tujuan, String status, String nama_barang, long id_pesanan){
        super(alamat_tujuan, status, id_pesanan);
        this.nama_barang = nama_barang;
    }

    public String getNama_barang(){
        return nama_barang;
    }

    public void setNama_barang(String nama_barang){
        this.nama_barang = nama_barang;
    }

    public String toString(){
        String x = "\nID Pesanan : "+this.getId_pesanan()+
                "\nNama Barang : "+this.getNama_barang()+
                "\nAlamat Tujuan : "+this.getAlamat_tujuan()+
                "\nStatus :"+this.getStatus();
        return x;
    }
}
