# Emissoras-Públicas-de-Rádio-e-Televisão-em-Todo-Mundo
Fazendo uma lista em ordem alfabética de emissoras públicas de rádio e televisão em todo o mundo.

Herbert Barbosa Ferreira

import java.util.*;

public class EmissorasPublicas {
    // Classe para armazenar as informações das emissoras
    static class Emissora {
        String nome;
        String pais;
        String tipo; // Pode ser "Rádio" ou "Televisão"

        Emissora(String nome, String pais, String tipo) {
            this.nome = nome;
            this.pais = pais;
            this.tipo = tipo;
        }

        @Override
        public String toString() {
            return "Emissora: " + nome + ", País: " + pais + ", Tipo: " + tipo;
        }
    }

    public static void main(String[] args) {
        // Criando uma lista de emissoras públicas
        List<Emissora> emissoras = new ArrayList<>();

        // Adicionando algumas emissoras públicas à lista
        emissoras.add(new Emissora("BBC", "Reino Unido", "Televisão"));
        emissoras.add(new Emissora("Rádio France", "França", "Rádio"));
        emissoras.add(new Emissora("PBS", "Estados Unidos", "Televisão"));
        emissoras.add(new Emissora("RTP", "Portugal", "Televisão"));
        emissoras.add(new Emissora("CBC", "Canadá", "Televisão"));
        emissoras.add(new Emissora("NHK", "Japão", "Televisão"));
        emissoras.add(new Emissora("ABC", "Austrália", "Televisão"));
        emissoras.add(new Emissora("TVE", "Espanha", "Televisão"));
        emissoras.add(new Emissora("CBC Radio", "Canadá", "Rádio"));
        emissoras.add(new Emissora("Rádio Nacional de España", "Espanha", "Rádio"));

        // Imprimindo as emissoras na tela
        System.out.println("Lista de Emissoras Públicas:");
        for (Emissora emissora : emissoras) {
            System.out.println(emissora);
        }
    }
}