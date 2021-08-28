# TESTE-ARTESANATOO
TESTE
  using System;
using System.Collections.Generic;
using DIO.artesanato.Interfaces;

namespace DIO.artesanato
{
	public class artesanatiRepositorio : IRepositorio<artesanato>
	{
        private List<artesanato> listaSerie = new List<artesanato>();
		public void Atualiza(int id, artesanato objeto)
		{
			listaartesanato[id] = objeto;
		}

		public void Exclui(int id)
		{
			listaartesanato[id].Excluir();
		}

		public void Insere(Serie objeto)
		{
			listaartesanato.Add(objeto);
		}

		public List<Serie> Lista()
		{
			return listaartesanato;
		}

		public int ProximoId()
		{
			return listaartesanato.Count;
		}

		public artesanato RetornaPorId(int id)
		{
			return listaartesanato[id];
		}
	}
}
    }
}
