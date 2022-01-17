package TULIPKU;

public class Pelanggan extends Orang{
    private Pesanan pesanan[] = new Pesanan[100];
    private long id_pelanggan;
    private String alamat_pelanggan;
    private int jml_pesanan;

    public Pelanggan(String nama, long no_telp , String alamat_pelanggan, long id_pelanggan, String username, String password){
        super.setNama(nama);
        super.setNo_telp(no_telp);
        super.setPassword(password);
        super.setUsername(username);
        this.alamat_pelanggan = alamat_pelanggan;
        this.id_pelanggan = id_pelanggan;
    }

    public long getId_pelanggan(){
        return id_pelanggan;
    }

    public void setId_pelanggan(long id_pelanggan){
        this.id_pelanggan = id_pelanggan;
    }

    public String getAlamat_pelanggan(){
        return alamat_pelanggan;
    }

    public void setAlamat_pelanggan(String alamat_pelanggan){
        this.alamat_pelanggan = alamat_pelanggan;
    }

    public void create_Pesanan(Pesanan P){
        if(getjml_pesanan()<100){
            pesanan[getjml_pesanan()] = P;
            setjml_pesanan(getjml_pesanan() + 1);
        }else{
            System.out.println("Pesanan Penuh !!!");
        }
    }

    public Pesanan getPesanan(int index) {
        return pesanan[index];
    }

    public boolean removePesanan(long id_pesanan){
        for (int j = 0; j < getjml_pesanan(); j++) {
            if (pesanan[j].getId_pesanan() == id_pesanan){
                if (j== 0){
                    pesanan[0] = null;
                    for (int k = 0; k < getjml_pesanan()-1; k++) {
                        pesanan[k] = pesanan[k+1];
                    }
                    pesanan[getjml_pesanan()] = null;
                    setjml_pesanan(getjml_pesanan() - 1);
                    return true;
                } else if(j == getjml_pesanan()){
                    pesanan[j] = null;
                    setjml_pesanan(getjml_pesanan() - 1);
                    return true;

                }else{
                    pesanan[j] = null;
                    for (int k = j; k < getjml_pesanan()-1; k++) {
                        pesanan[k] = pesanan[k+1];
                    }
                    pesanan[getjml_pesanan()] = null;
                    setjml_pesanan(getjml_pesanan() - 1);
                    return true;
                }

            }
        }
        return false;
    }
    public String toString(){
        String x = "\nID Pelanggan : "+this.getId_pelanggan()+
                "\nNama Pelanggan : "+this.getNama()+
                "\nNo Telepon : "+this.getNo_telp()+
                "\nAlamat :" +this.getAlamat_pelanggan();
        return x;
    }

    public int getjml_pesanan() {
        return jml_pesanan;
    }

    public void setjml_pesanan(int jml_pesanan) {
        this.jml_pesanan = jml_pesanan;
    }
}
