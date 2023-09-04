# PR1-miapo
pr1
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace PR3
{
    // класс верхнего уровня
    public class polka
    {
        IVehicle m_Vehicle;
        // конструктор, в который передается объект, нижнего уровня
        // поддерживающий интерфейс IVehicle
        public polka(IVehicle vehicle)
        {
            this.m_Vehicle = vehicle;
        }
        // методы задания команд объекту нижнего уровня
        // команда ускориться
        public void Attack()
        {
            m_Vehicle.Attack();
        }
        // команда затормозить
        public void Defend()
        {
            m_Vehicle.Defend();
        }
        public void Run()
        {
            m_Vehicle.Run();
        }
    }

